# Measurement ruleset

This document is the normative description of how the numbers in this
repository are produced. Every published figure carries the ruleset version it
was computed under (e.g. `ruleset 0.4.0` in the README header and in each
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

## The route catalog

Which routes are measured is itself data, not a given. No route enters the
catalog without a nameable `issuer` and an `evidence` record; the build fails
otherwise. Each route also carries a **tier**, and a tier states *where the
route comes from* — it is not a quality rating and it never weights a figure:

| Tier | Meaning |
|:--|:--|
| 1 | Formally registered (IANA registry or RFC). The control group. |
| 2 | Strong issuer of the AI era (Linux Foundation, Google, Microsoft, Anthropic, …). |
| 3 | Convention with demonstrable consumers. |
| 4 | Single issuer, dormant, or speculative. **A zero here is a measurement, not a gap.** |

Tier 4 is deliberately kept populated: a route that nobody implements is a
finding, and it can only be reported if it was asked for.

Routes that are watched but not yet measured appear as *under observation* in
each release and carry no numbers. They are **not requested in the monthly
run**; a monthly field probe on 1,000 panel sources and the discovery runs
request them, and nothing from those requests is counted or published. The
discovery runs visit domains outside the frame and additionally request a short
list of routes named in the README ("Requested only by discovery runs"). A
watched route is promoted to measured when it is found at three
or more independent organisations. Every addition and removal since the first
run is recorded in [ROUTES-CHANGELOG.md](ROUTES-CHANGELOG.md).

## Classification states

Every (domain, route) pair receives exactly one state:

| State | Meaning |
|:--|:--|
| `present` | A file exists and passes the form checks below. |
| `alias` | The same body as another catalogued path of the same host (see *Order of judgement*) — the file exists, but it is not counted twice. |
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
  (`via: header`) when no file-based judgement succeeded. Since v0.4.0 a
  parseable JSON body at `/.well-known/tdmrep.json` without any spec field
  counts as `present` (`via: file-unset`, not spec-conforming) unless it is
  the host's catch-all or a JSON error page. The rule is literal: any such
  body counts, including a policy file of another vocabulary, which is why
  both figures are reported.
- **RSL** fixes no path for the licence file. `/rsl.xml` is measured as a
  route like any other; alongside it we report how many organisations declare
  a licence with a `License:` line in their `robots.txt` and how many of those
  point to `/rsl.xml` — a second figure next to the route, which does not
  change the route's share.

**Order of judgement.** Form check, catch-all and alias can all apply to the
same response, so their precedence is fixed and it matters: form checks
first, then catch-all, then alias. A body that appears on **three or more**
catalogued paths of one host is a catch-all and every one of those paths is
`soft404` — it is never read as three aliases. Only when exactly two paths
share a body does the alias rule apply, and then the path that comes **first
in catalog order** is the primary and keeps its own verdict; the other
becomes `alias`. Sameness is decided on the byte length plus the first 300
bytes of the body, not on a full byte comparison — a cheap test that is
deliberately slightly generous, because the failure it guards against
(counting one file two or three times as adoption) is worse than the one it
risks.

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

What the interval estimates is the share among the **observed** hosts of the
frame, and it covers **sampling variation only**. It does not cover the choice
of frame, and it does not cover measurement error: a route whose observed base
is thinned by bot walls has a narrow interval around a share drawn from
whichever hosts let us in. Where walls are unevenly distributed — and they
concentrate in the popular ranks — that is the larger uncertainty, and no
interval on this page expresses it.

## Sample frame

A frozen, stratified frame drawn from the Tranco list (permanent list ID in
each `data/*.json`) and the Chrome UX Report country top lists (de/at/ch/it/
global). The current frame is **2026-Q3**: Tranco `645KX` (2026-08-11,
957,354 domains after eTLD+1) and CrUX `202607`, drawn with the fixed seed
`20260811`, so the draw is reproducible from the sources alone.

| Stratum | Size | Recipe |
|:--|--:|:--|
| `dach` | 8,000 | CrUX de 5,000 + at 1,500 + ch 1,500, best size classes first |
| `italien` | 3,000 | CrUX it, best size classes first |
| `global-spitze` | 5,000 | Tranco rank order ∩ CrUX-global classes ≤ 10,000 — rank orders, CrUX decides membership |
| `global-breite` | 10,000 | Tranco ranks 5,000–100,000, every k-th |
| `long-tail` | 4,000 | Tranco ranks 100,000–1,000,000, every k-th |

CrUX `rank` is a **size class** (1000, 5000, 10000, …), not an exact rank;
inside the boundary class a seeded shuffle decides, not the alphabet and not
the file order. A CrUX country list means "used there", not "from there", so
international brands without a country domain are in `dach` and `italien` by
design — the frame measures what users in a market meet. Every domain belongs
to exactly one stratum; on collision the precedence is
`dach > italien > global-spitze > global-breite > long-tail`, and the losing
stratum refills from its own source, which is why target equals actual despite
7,616 collisions at build time. The precedence follows the priority of the
questions: the market question may take a domain from the top-rank question,
never the other way round, because otherwise the smallest stratum would be the
most perforated. The frame is deduplicated at the registrable-domain level; each
domain is measured at most once per quarter, except the panel's domains, which
are measured every month. The seed lists themselves are **not** published (see
below).

**How the frame is split.** From the 30,000 registrable domains, a **panel** of
1,000 was drawn proportionally per stratum (seeded sampling, so the draw is
reproducible from the frame). The remaining 29,000 are shuffled per stratum with
the same seeded generator and dealt round-robin into **three blocks a, b, c**
(9,667 / 9,667 / 9,666 domains), so each block carries every stratum in the
same proportion. **Since October 2026 the panel has 10,000 domains** — a third
of the frame: 9,000 further domains were drawn proportionally per stratum from
the three blocks with a separate seeded stream, and the original 1,000 stay
inside it. One block is measured per month together with the panel: **a** in
the first month of the quarter (September 2026), **b** in the second, **c** in
the third; a block domain that belongs to the panel is measured once, as part
of the panel. A monthly run is therefore the panel plus the rest of the month's
block (October 2026: 16,597 domains); its figures describe *coverage* of the
frame, the panel's figures describe *change*. Attribution for
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

Since September 2026 one run per month measures the **panel** (fixed sources,
measured every month: 1,000 in September 2026, 10,000 since October 2026)
together with one rotating **block** of the frame (each block source measured
once per quarter). The published panel figures are computed as a **subset of
that run**: the same raw archives, filtered to the frozen panel list; the
finding records the list's hash and how many records it kept (`subset`).
Until December 2026 the original 1,000-source panel is computed as a second
subset of the same run and published as its own series (`panel1000-YYYY-MM`),
because it is the only series that reaches back to August 2026. Only
panel-to-panel comparisons within one series are trends — the 10,000 and the
1,000 series are never chained, and block figures describe coverage, not
change.

## The quarterly roll-up

At the end of a quarter the three monthly runs are combined into one figure
over the **whole** frame instead of a third of it. The combination is not a
concatenation: each monthly run measured the panel *and* its block, so
appending the three runs would count 32,001 domains for a frame of 30,000 and
put triple weight on 1,000 unusually well-maintained hosts, biasing every
share upward.

**The panel is therefore counted exactly once.** Each block is taken from its
own run, and the panel from a single nominated month (by default the last,
because that release carries the number). The roll-up states which month's
panel it used; a quarterly figure is comparable only to another quarterly
figure over the same frame.

## Data files and their status

Each release carries the data files of its month: `panel-YYYY-MM` (the
panel, the trend series — 10,000 sources since October 2026),
`panel1000-YYYY-MM` (the original 1,000-source panel as its own series, from
October to December 2026) and `monat-YYYY-MM-block-x` (the month's run, block
plus panel, the coverage series). Every file states
its own completeness in `measurement_window`: `started` and
`completed` are the first and last measuring tick, `status` is
`final` when the run's queue was empty at evaluation time (otherwise
`partial` with `queue_open`). Only final files are released.
**Numbers in a released file are never changed.** Metadata may be added later
(as on 05.09.2026, when `completed` and `status` were introduced);
the Zenodo snapshot of a version holds the files exactly as of that tag, so a
DOI always cites a fixed state.

**State breakdown per route (from v2026.10).** Each route row also carries the
seven classification states it was built from — `present`, `alias`,
`soft404`, `absent`, `blocked`, `disallowed`, `unreachable` (as `states` in
the JSON, as `state_*` columns in the CSV). With them, `n` stops being a bare
number: the first four sum to `n` and `present` is the numerator, while the
last three are the part of the sample that never answered the question. A
reader can therefore see how much of a host set was inspected at all, and
recompute any share under a different denominator.

Files released before v2026.10 do **not** carry these fields and are not
back-filled. Nothing about their numbers would change — only fields would be
added — but a published file that quietly gains content is no longer the file
someone cited.

## Verification

Every published number — panel **and** block run alike — is re-derived from
the checksummed raw archives by an independent re-evaluation before release
(manifest hash check → re-classify →
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
| 0.4.0 | 2026-10-01 | A parseable JSON body at `/.well-known/tdmrep.json` that carries no spec field but is **not the host's catch-all** now counts as `present` with the flag `via: file-unset` — an implementation with an unset rule, rather than a forged page. Both figures are reported (`present` and `present − viaFileUnset`); the old figure remains derivable for every run. Committed in https://github.com/w3c-cg/tdm-reservation-protocol/issues/62. Measured effect on the September archive: 28 → 29; on the October run: 43 under both rules. The clause "not the host's catch-all" does most of the work — the empty-array files this rule was written for are served on 13 paths each and stay excluded. |

Errors we find in our own measurement are documented in the version history
above rather than silently corrected; the private repository keeps the full
errata trail.
