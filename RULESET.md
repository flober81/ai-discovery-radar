# Measurement ruleset

This document is the normative description of how the numbers in this
repository are produced. Every published figure carries the ruleset version it
was computed under (e.g. `ruleset 0.3.1` in the README header and in each
`data/*.json`). When a rule changes, the version changes, affected numbers are
recomputed and republished under the new version, and the change is recorded
here — numbers from different ruleset versions are not silently comparable.

The reference implementation and the raw response archives live in a private
companion repository (see "Why the raw data is private" below). This document
is written so that the measurement can be re-implemented from it alone.

## What is measured

For each domain in the sample, a fixed catalog of well-known routes (the
`route` column of the data files, e.g. `/robots.txt`, `/llms.txt`,
`/.well-known/tdmrep.json`) is fetched over HTTPS at the registrable domain's
apex, at a polite rate, honouring `robots.txt`:

- If robots rules disallow a path for our user agent, the path is **not
  fetched** and recorded as `disallowed`.
- If a host requests a crawl delay beyond our per-run budget, the path is
  recorded as `notmeasured` (nobody refused us; we simply did not measure).
- The user agent identifies the project and links to this repository.
  Opt-out instructions are in `SECURITY.md`; opted-out domains are removed.

## Classification states

Every (domain, route) pair receives exactly one state:

| State | Meaning |
|:--|:--|
| `present` | A file exists and passes the form checks below. |
| `alias` | Byte-identical to the same file at another catalogued path of the same host — exists, but is not counted twice. |
| `soft404` | The server said 200 but delivered something else (an HTML page where none belongs, a text error page, a catch-all response, or syntactically broken JSON). Counted as *not adopted*, reported separately. |
| `absent` | An honest 404/410 or an empty body. |
| `blocked` | A bot wall (recognised by response-body signatures), a rejecting status (401/403/429/5xx), or a timeout. **Never counted as "not adopted".** |
| `disallowed` | robots.txt forbids us the path. **Never counted as "not adopted".** |
| `unreachable` | DNS/TLS/connection failure at host level. |

### Form checks for `present`

- **JSON routes** must parse and carry at least one required key of their
  specification (e.g. `protocolVersion`/`skills`/`capabilities` for
  agent-card). The canonical **array form** counts (a spec-conforming
  `[{...}]` wrapper is unwrapped — v0.3.1). If the stored body was truncated
  by the pipeline, a key-pattern fallback is used instead of `JSON.parse`
  (v0.3.2).
- **Text routes** with a 200 but a short error-looking body ("not found",
  "forbidden", …) are `soft404`; whitespace-only bodies are `absent`.
- A body served identically on ≥3 catalogued paths of the same host is a
  **catch-all** response and every such path is `soft404`.
- **Redirects are followed** (standard fetch semantics, up to 20 hops),
  including cross-host redirects; the final URL is recorded as provenance
  alongside each result. All checks above apply to the **final** response —
  a route that redirects to an HTML landing page therefore ends up as
  `soft404`, and a route redirecting to the same document as another
  catalogued path is caught by the alias/catch-all rules and not counted
  twice.
- **TDMRep** may be declared via the `tdm-reservation`/`tdm-policy` response
  header on any resource of the host; a valid header yields `present`
  (`via: header`) when no file-based judgement succeeded.

### Bot walls

Detected on the **full** response body at fetch time (5.66 % of wall markers
sit beyond 2 KB) via vendor-specific body signatures, after decoding numeric
HTML entities (one vendor encodes its own markers — v0.3.2 lesson, see
version history). The wall verdict is stored as a flag and survives archive
trimming.

## The denominator (v0.3.0)

Adoption shares are computed **only over observed states**:

```
share(route) = present / (present + alias + soft404 + absent)
```

`blocked`, `disallowed`, `unreachable` and `notmeasured` are excluded from
the denominator entirely. Rationale: a host that refused the door, or that we
were not allowed to ask, is not evidence of non-adoption — counting it as
such would systematically bias shares downward, and unevenly so (walls
concentrate in popular ranks). Each route therefore has its own `n` (the
observed base), published alongside the share.

## Confidence intervals

95 % intervals are Wilson score intervals on (count, n) per route. They are
intervals for *this sample frame*, not for "the web".

## Sample frame

A frozen, stratified frame drawn from the Tranco list (permanent list ID in
each `data/*.json`) and the Chrome UX Report country top lists (de/at/ch/it/
global). The frame is deduplicated at the registrable-domain level; each
domain is measured at most once per quarter (monthly panel: three times). The
seed lists themselves are **not** published (see below). Attribution for
Tranco, CrUX and Majestic is in the README ("Sample attribution").

## Why the raw data is private

Raw archives contain response bodies; two catalogued routes
(`security.txt`, `humans.txt`) routinely carry **personal data** (contact
addresses, names). Publishing per-domain results would also turn a neutral
measurement into a public register of who blocks whom. We therefore publish
aggregates only; the private archives are checksummed (SHA-256 manifests) and
every published figure is reproducible from them by the verification step
described below.

## Panel and monthly run

Since September 2026 one run per month measures the **panel** (1,000 fixed
sources, measured every month) together with one rotating **block** of the
frame (about 9,700 sources, each measured once per quarter). The published
panel figures are computed as a **subset of that run**: the same raw archives,
filtered to the frozen panel list; the finding records the list's hash and
how many records it kept (`subset`). Only panel-to-panel comparisons are
trends — block figures describe coverage, not change.

## Verification

Every published number is re-derived from the checksummed raw archives by an
independent re-evaluation before release (manifest hash check → re-classify →
byte-compare against the published aggregate). The README tables and the
`data/*` files are **generated** from the same verified aggregate; automated
drift guards fail the build when any published copy differs from a fresh
generation.

## Version history

| Version | Date | Change |
|:--|:--|:--|
| 0.2.0 | 2026-08-10 | First coherent ruleset after the pilot audit: seven states, robots-respect, catch-all and alias detection, wall detection at fetch time. |
| 0.3.0 | 2026-08-17 | **Denominator = observed states only.** Previously `blocked`/`disallowed`/`unreachable` sat in the base where they could never reach the numerator — arithmetically "not adopted", contradicting the classifier's own contract. Affected roughly one fifth of every denominator; the August line was republished. |
| 0.3.1 | 2026-08-21 | JSON schema check unwraps the **canonical array form** (TDMRep: `[{"tdm-reservation":1}]`). 29 valid files had been misclassified as `soft404` and resurfaced as header-only declarations. |
| 0.3.2 | 2026-08-22 | Archive truncation now marks itself, and readers of older archives infer the mark. The 2 KB archive trim silently cut large JSON bodies; the classifier parsed the fragment, failed, and judged `soft404` — valid files (systematically the *large* ones) were counted as forgeries. Additionally: bot-wall signatures are matched after decoding numeric HTML entities — one major vendor's wall had never been recognised in 14 months, so **no vendor breakdown of walls is published for runs before this version**. |

Errors we find in our own measurement are documented in the version history
above rather than silently corrected; the private repository keeps the full
errata trail.
