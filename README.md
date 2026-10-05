# ai-discovery-radar

**English** · [Deutsch](README.de.md) · [Italiano](README.it.md)

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22178282.svg)](https://doi.org/10.5281/zenodo.22178282)

**Method:** how these numbers are measured, classified and verified is documented in the [Technical Report v1.0](https://doi.org/10.5281/zenodo.22769680) (CC BY 4.0). Read it before citing a share.

> **Found this in your server logs?** You can opt out in one line — see
> [Opt out](#opt-out) below. No account, no contact, no reason required.
>
> <!-- LAST:START -->
> **How often we visit:** about **16,600 sources (domains) per month**: the 10,000-source panel every month, plus a rotating block of the ~30,000-source frame, each block source at most once per quarter. Once a month, 1,000 of the panel sources are also asked for the routes under observation.
>
> In addition, small discovery runs visit popular domains outside the frame — at most about 2,000 a day — with the routes in the tables below plus the short list under “Requested only by discovery runs”. Their results are never published; the same opt-out applies.
> <!-- LAST:END -->

A radar of the AI discovery files on the public web: which routes exist
(`robots.txt`, `llms.txt`, `ai-catalog.json`, …), how widely they are used, and
whether they can be fetched at all. Every blip is a measurement, not an opinion.

## The radar

<!-- RADAR:START -->
_Run **panel-2026-10** · 8636 reachable hosts (8636 registrable domains) · ruleset 0.4.0_

| Route | Purpose | Publisher | n | Adoption | 95% CI | Trend |
|:--|:--|:--|--:|--:|:--|:-:|
| `/robots.txt` | Which parts of a site automated clients may enter | IETF | 7590 | 83.72% | 82.9–84.5 | — |
| `/sitemap.xml` | An index of every address a website offers | sitemaps.org | 6890 | 54.40% | 53.2–55.6 | — |
| `/llms.txt` | A table of contents for language models | Answer.AI | 6635 | 14.11% | 13.3–15.0 | — |
| `/.well-known/security.txt` | Where to report a security vulnerability | IETF | 6862 | 8.16% | 7.5–8.8 | — |
| `/.well-known/oauth-authorization-server` | How the service that grants access rights works | IETF | 6782 | 6.56% | 6.0–7.2 | — |
| `/.well-known/oauth-protected-resource` | Where a client obtains authorization for access | IETF | 6779 | 6.08% | 5.5–6.7 | — |
| `/llms-full.txt` | A whole website's content in a single file | Answer.AI | 6639 | 4.34% | 3.9–4.9 | — |
| `/.well-known/gpc.json` | Whether the site honors the data-sharing opt-out | W3C Global Privacy Control | 6800 | 2.84% | 2.5–3.3 | — |
| `/security.txt` | Where to report a vulnerability, at the site root | IETF | 7050 | 1.21% | 1.0–1.5 | — |
| `/.well-known/traffic-advice` | Whether a caching proxy may prefetch pages | Google (Private Prefetch Proxy) | 6760 | 0.99% | 0.8–1.3 | — |
| `/rsl.xml` | The license terms under which content may be used | RSL Collective | 6353 | 0.66% | 0.5–0.9 | — |
| `/.well-known/openid-configuration` | Where and how to sign in at this domain | OpenID Foundation | 6771 | 0.37% | 0.3–0.5 | — |
| `/.well-known/tdmrep.json` | Whether text and data may be mined automatically | W3C TDM Reservation Protocol CG | 6796 | 0.37% | 0.2–0.5 | — |
| `/ai.txt` | Which content is withheld from AI training | Spawning | 6606 | 0.27% | 0.2–0.4 | — |
| `/.well-known/api-catalog` | An index of the interfaces a domain offers | IETF | 6792 | 0.25% | 0.2–0.4 | — |
| `/openapi.json` | A description of an interface for other programs | OpenAPI Initiative | 6368 | 0.19% | 0.1–0.3 | — |
| `/.well-known/ai-catalog.json` | What content and services a domain offers AI agents | AI Catalog WG (Linux Foundation), Google, Microsoft | 6733 | 0.09% | 0.0–0.2 | — |
| `/.well-known/ai-plugin.json` | Instructions for a chatbot to operate a service | OpenAI | 6589 | 0.09% | 0.0–0.2 | — |
| `/.well-known/mcp.json` | Which tool servers a domain provides for AI | Model Context Protocol | 6726 | 0.07% | 0.0–0.2 | — |
| `/.well-known/host-meta` | Pointers to a domain's other points of information | IETF | 6783 | 0.06% | 0.0–0.2 | — |
| `/.well-known/agent-card.json` | What a software agent can do and how to address it | A2A Project (Linux Foundation) | 6733 | 0.03% | 0.0–0.1 | — |
| `/.well-known/ai.txt` | The same AI usage rules in the well-known folder | Spawning | 6620 | 0.03% | 0.0–0.1 | — |
| `/.well-known/did.json` | A domain's provable identity without a central party | W3C | 6704 | 0.03% | 0.0–0.1 | — |
| `/swagger.json` | An interface description under the older file name | SmartBear (Swagger) | 6302 | 0.03% | 0.0–0.1 | — |
| `/.well-known/llms.txt` | A table of contents for language models, in well-known | Answer.AI | 6589 | 0.02% | 0.0–0.1 | — |
| `/.well-known/webfinger` | Who is behind an address at this domain | IETF | 6632 | 0.02% | 0.0–0.1 | — |
| `/mcp.json` | A machine-readable list of a site's MCP endpoints, at the root | Anthropic et al. (MCP) — root-path variant not specified | 6301 | 0.02% | 0.0–0.1 | — |
| `/.well-known/agent.json` | An agent's capabilities, under the older file name | A2A Project (Linux Foundation) | 6729 | 0.01% | 0.0–0.1 | — |
| `/.well-known/dnt-policy.txt` | A pledge not to track visitors across sites | EFF | 6798 | 0.01% | 0.0–0.1 | — |
| `/.well-known/mcp-server` | Where to reach a domain's tool server | IETF (individual draft) | 6743 | 0.01% | 0.0–0.1 | — |
| `/.well-known/openapi.json` | An interface description in the well-known folder | OpenAPI Initiative | 6709 | 0.00% | 0.0–0.1 | — |
| `/.well-known/openid-federation` | Which federation a party provably belongs to | OpenID Foundation | 6777 | 0.00% | 0.0–0.1 | — |
| `/.well-known/x402.json` | The price and payment route for machine requests | Coinbase, Cloudflare | 6709 | 0.00% | 0.0–0.1 | — |
| `/ai-plugin.json` | The same chatbot instructions, at the site root | OpenAI | 6305 | 0.00% | 0.0–0.1 | — |

Adoption is the share of sources we were actually allowed to inspect that
served the route, with a 95% Wilson interval. Sources that turned us away
(bot wall), forbade the fetch via robots.txt, or could not be reached are
counted and reported separately — but a non-answer is not a "no", so they
are not part of the denominator.
**`n` is the number of hosts on which this route was actually probed. It
differs between routes, so each row has its own denominator and the rows
are not directly comparable with one another.**
No trend arrow in this edition. The previous runs cover a different part of the frame, so an arrow between them would partly measure the change of population rather than the change on the web. From December the quarterly roll-up compares like with like — the whole frame against the whole frame — and the arrow returns there.
Of the 1535 `/llms.txt` files found in the whole monthly run `monat-2026-10-block-b` (panel and block), 517 (33.7%) carry the marks of a generator — a self-declared producer or wording shared with other sites; the producers that name themselves are content-management plugins (largest: yoast seo 112, all in one seo 29, rank math seo 19). The adoption figure above counts files, and that stays right: a file rolled out by a plugin exists and is read. This footnote answers the other question — how much of the number is a decision. It is an indication for this run, not a published rate.
Of the 469 `/llms-full.txt` files found in the whole monthly run `monat-2026-10-block-b` (panel and block), 343 (73.1%) carry the marks of a generator — a self-declared producer or wording shared with other sites. The adoption figure above counts files, and that stays right: a file rolled out by a plugin exists and is read. This footnote answers the other question — how much of the number is a decision. It is an indication for this run, not a published rate.

### Notes on this run

- From October 2026 the panel has 10,000 sources (a third of the frame). The earlier 1,000-source panel continues inside it as a subset until December 2026 and is published as its own series (`data/panel1000-YYYY-MM.*`); the two series are never chained.
- Of the 238 panel sources that carried Cloudflare's managed robots.txt block in September, those using the marker form still carry a block in 11 of 149 readable files (7.38%, 95% CI 4.2–12.7); those using the preamble-only form in 38 of 38 (100%, 95% CI 90.8–100.0).
- 47 files could not be read in October (20.09% of the pair, against 20.15% across the panel) and 4 hosts were unreachable.
- We give no combined rate: it would hide that one notation changed while the setting stayed.
- Delivers Markdown when Markdown is preferred: 154 of 6,509 organisations (2.37%, 2.0–2.8).
- Announcing a Markdown version beforehand is rarer: `rel="describedby"` 9, `rel="alternate" type="text/markdown"` 2 (a lower bound — only HTTP Link headers are countable).
- A single request cannot tell whether a server negotiates or always serves Markdown.
- Because our one home-page request prefers Markdown, 154 home pages answered without an HTML head; their link relations are not read.
- TDMRep under ruleset 0.4.0: 25 on the panel under the new rule, 25 under the old one (see the version history in RULESET.md).
- 2 organisations declare a licence in robots.txt (`License:`); 1 of them points to `/rsl.xml`.
- 3 organisations announce llms.txt in robots.txt under a path other than the root; the file belongs at the root, so they are not counted.
- DNS: of 10,000 panel sources, 0 publish a specification-conformant `_agent` record and 0 an `_mcp` record that can be told apart from wildcard or verification answers.
- `/.well-known/ai-catalog.json`: in the fixed 1,000-source panel 0 of 675 in September and 0 of 676 in October; in the 10,000-source panel 6 of 6,733 (0.09%). Lighthouse has checked the file since 2026.



## Under observation (24)

**Confirmed** — registered (IANA) or RFC, barely seen in the field yet:

- `/.well-known/nostr.json` — Nostr Developer Community (NIP-05). Proof that a public key belongs to a name at this domain
- `/.well-known/vacation-rental.json` — Vacation Rental Protocol (single registrant). Discovery document for cryptographically signed stay offers
- `/.well-known/xregistry` — xRegistry Authors (CNCF Sandbox). Entry point of an extensible registry for schemas and events
- `/.well-known/host-meta.json` — IETF. JSON twin of the host-meta pointers
- `/.well-known/open-resource-discovery` — SAP SE (Open Resource Discovery). An entry point listing the APIs and events a system exposes for discovery

**Emerging** — field signals or drafts, no registration yet:

- `/.well-known/atproto-did` — AT Protocol (Bluesky). Resolves a domain handle to a decentralized identity
- `/server-card.json` — no nameable publisher (circulating agent spec). A proposed self-description card for agent-facing servers
- `/product.xml` — no publisher — emerging commerce convention. Product listings that shops link for machine readers
- `Signposting (Link header: describedby/cite-as/linkset)` — FAIR Signposting Profile (scholarly repository community). Machine-readable pointers from scholarly pages to their metadata and full texts
- `/.well-known/jwt-vc-issuer` — IETF (OAuth WG, draft stage). Where a verifier finds an issuer's keys for verifiable credentials
- `/.well-known/ai` — IETF draft (AI Discovery Endpoint). A proposed machine-readable capability description for AI agents
- `_agent (DNS TXT record, no HTTP route)` — IETF draft (Agent Identity and Discovery, AID). A DNS record proposing agent identity discovery
- `Content-Usage (robots.txt directive + HTTP header, no path)` — IETF AIPREF WG (draft-ietf-aipref-attach, WG-adopted, Standards Track). A directive stating what AI may do with the content
- `Schemamap (robots.txt directive; target URL free, conventionally /schema.txt)` — SCHEMA.TXT (specification on GitHub). A directive pointing machines to a site's schema map
- `/.well-known/did-configuration.json` — Decentralized Identity Foundation (DIF). Proof linking a domain to decentralized identifiers
- `_apertoid (DNS TXT record, no HTTP route)` — ApertoID (single vendor). A DNS record for an emerging open-identity proposal
- `_x402 (DNS-TXT) + /.well-known/x402` — Individual draft (W. Hawkins) for the Coinbase/Cloudflare x402. DNS and web discovery of x402 payment endpoints
- `_agents / AIDISCA+AIINDEX (new DNS RR types)` — Verisign (individual draft). Proposed DNS record types for agent discovery
- `Link rel=client-ranges (HTTP Link header)` — Individual draft (Google/Ericsson authors). A header pointing clients to declared IP ranges
- `Agentmap (robots.txt directive; target URL free)` — AI Catalog Working Group (Linux Foundation) — Agentic Resource Discovery spec. A robots.txt line pointing machines to a site's AI resource catalog
- `Archive-Embargo / Embargo-Allow (robots.txt directives, no path)` — Individual draft (M. Nottingham, M. Thomson — HTTP WG environment). robots.txt lines controlling when archived copies of a site may be published
- `/agents.md` — Shopify (Plattform-Vorgabe) sowie die AGENTS.md-Konvention aus Code-Ablagen. How a site describes itself to AI agents
- `/.well-known/ucp` — Universal Commerce Protocol (UCP Tech Council). Which commerce capabilities a merchant offers agents
- `/.well-known/agent-skills/index.json` — Cloudflare (Agent Skills Discovery RFC, Status Draft). Which agent skills a domain offers, with version and digest

_Observed routes are not requested in the monthly run. Our discovery runs (see below) and a monthly field probe on 1,000 of the panel sources request them, and count nothing from them for this page. Each entry names its promotion criterion in the lab._

### Requested only by discovery runs (20)

- `/.well-known/api-catalog.json`
- `/.well-known/http-message-signatures-directory`
- `/.well-known/signature-agent-card`
- `/.well-known/agent-trust`
- `/.well-known/agent-trust-keys`
- `/.well-known/aicp`
- `/.well-known/ahp.json`
- `/.well-known/ahp/reputation`
- `/.well-known/botcentral.txt`
- `/.well-known/llm-context`
- `/.well-known/acp.json`
- `/.well-known/terms.txt`
- `/.well-known/ai.json`
- `/.well-known/ard.json`
- `/llms-small.txt`
- `/llms-ctx.txt`
- `/llms-ctx-full.txt`
- `/trust.txt`
- `/.well-known/trust.txt`
- `/.well-known/agent`
<!-- RADAR:END -->
**What we request.** The lists above are the complete list of routes we
request: the measured routes in every monthly run; the routes under
observation only in the monthly field probe on 1,000 panel sources and in the
discovery runs; the routes under “Requested only by discovery runs” only in
those. Three additions: your home page, once, to read its `<link rel>`
announcements (the page itself is discarded); when files on your own domain
point to another file there — a link in your `robots.txt`, say — we may fetch
that referenced file once, at most one such follow-up per domain and run, under
the same `robots.txt` rules; and three DNS records per domain (`_agent`, `_mcp`,
`_index._agents`): plain name-service lookups that never touch your web server.
Nothing we fetch is published as content — only counts and shares per route,
and nothing at all from the field probe or the discovery runs.

**How a route gets into the table.** It needs a nameable publisher or a
documented consumer that reads it — not merely a format being passed around
somewhere. The publisher is in the table so that every row can be checked on
its own. The purpose says what the file does on a server; it describes the
file, it does not judge it.

## How we measure

The measurement obeys your `robots.txt`, identifies itself honestly with this
repository as the sender, and works slowly and sparingly. Only public
configuration files meant for machines are fetched — no page content.

The figures above are the **October 2026 panel**: since October 2026 a
stratified panel of 10,000 sources — a third of the 30,000-source frame — is
measured every month; the earlier 1,000-source panel continues inside it as its
own series (see the notes below the table). This edition shows no trend arrow;
the note below the table says why. Every other source of the frame is measured
once per quarter. The **14-month
review** of AI directive adoption announced for the first monthly report is
published: [REVIEW-2025-2026.md](REVIEW-2025-2026.md) — eight Common Crawl
snapshots, June 2025 to July 2026: response headers of **3.6 million pages**
(2.7 million organisations), plus a separate scan of more than **270,000
robots.txt files**.

## Data files per month

The table above is the **panel**: 10,000 fixed sources (a third of the
frame), measured every month. Only panel against panel can show change, and
only within one series: until December 2026 the earlier 1,000-source panel is
published alongside as its own series — the only one that reaches back to
August 2026 — and the two series are never chained. Every month one **block**
of the wider 30,000-source frame is measured in the same run — the frame is
split into three blocks (a, b, c) that rotate through the quarter, so each
block source is visited once per quarter. Block **b** ran in October 2026. The
block run's purpose is coverage, not trend.

All series are published in [`data/`](data/): `panel-YYYY-MM.{json,csv}`,
`panel1000-YYYY-MM.{json,csv}` and `monat-YYYY-MM-block-x.{json,csv}`. Each file states when it was
measured and whether it is complete (`measurement_window.status`); how
the frame is split is defined in [RULESET.md](RULESET.md).

## Who runs this

The radar is operated by **Berger+Team**, a freelancer collective in South
Tyrol, Italy, alongside its work on [btlabs Core](https://btlabs.dev/en). The
measurement exists because that work needs numbers instead of assumptions:
which discovery routes are actually in use, and which are merely being
discussed. What is published here is what was measured — including the routes
that came back at zero.

## Opt out

No questions asked, no reason needed. Any one of these is enough:

1. Email **florian@berger.team** with the domain — you do not need a
   GitHub account for this, **or**
2. open an issue in this repository with the domain, **or**
3. put a `Disallow` rule for our token `ai-discovery-radar` in your `robots.txt` — this
   works without contacting us at all.

Excluded domains are skipped **before** any request is made. Contact,
corrections and the full policy: [SECURITY.md](SECURITY.md).

## Sample attribution

The domain sample is drawn from the [Tranco list](https://tranco-list.eu/)
(research ranking; our frozen frame references a permanent Tranco list ID) and
the [Chrome UX Report top lists](https://github.com/zakird/crux-top-lists)
(© Google, [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)).
Tranco itself aggregates several providers, including the Majestic Million
(© Majestic, [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/)).

## License

MIT — see [LICENSE](LICENSE).
