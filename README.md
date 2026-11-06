# ai-discovery-radar

**English** · [Deutsch](README.de.md) · [Italiano](README.it.md)

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22178282.svg)](https://doi.org/10.5281/zenodo.22178282)

**Method:** how these numbers are measured, classified and verified is documented in the [Technical Report v1.0](https://doi.org/10.5281/zenodo.22769680) (CC BY 4.0). Read it before citing a share.

> **Found this in your server logs?** You can opt out in one line — see
> [Opt out](#opt-out) below. No account, no contact, no reason required.
>
> <!-- LAST:START -->
> **How often we visit:** about **16,800 sources (domains) per month**: the 10,000-source panel every month, plus a rotating block of the ~30,000-source frame, each block source at most once per quarter. Once a month, 1,000 of the panel sources are also asked for the routes under observation.
>
> In addition, small discovery runs visit popular domains outside the frame — at most about 2,000 a day — with the routes in the tables below plus the short list under “Requested only by discovery runs”. Their results are never published; the same opt-out applies.
> <!-- LAST:END -->

A radar of the AI discovery files on the public web: which routes exist
(`robots.txt`, `llms.txt`, `ai-catalog.json`, …), how widely they are used, and
whether they can be fetched at all. Every blip is a measurement, not an opinion.

## The radar

<!-- RADAR:START -->
_Run **panel-2026-11** · 8603 reachable hosts (8603 registrable domains) · ruleset 0.4.0_

| Route | Purpose | Publisher | n | Adoption | 95% CI | Trend |
|:--|:--|:--|--:|--:|:--|:-:|
| `/robots.txt` | Which parts of a site automated clients may enter | IETF | 7602 | 84.94% | 84.1–85.7 | → |
| `/sitemap.xml` | An index of every address a website offers | sitemaps.org | 6828 | 54.51% | 53.3–55.7 | → |
| `/llms.txt` | A table of contents for language models | Answer.AI | 6567 | 14.76% | 13.9–15.6 | → |
| `/.well-known/security.txt` | Where to report a security vulnerability | IETF | 6805 | 8.38% | 7.7–9.1 | → |
| `/.well-known/oauth-authorization-server` | How the service that grants access rights works | IETF | 6716 | 6.64% | 6.1–7.3 | → |
| `/.well-known/oauth-protected-resource` | Where a client obtains authorization for access | IETF | 6713 | 6.26% | 5.7–6.9 | → |
| `/llms-full.txt` | A whole website's content in a single file | Answer.AI | 6556 | 4.51% | 4.0–5.0 | → |
| `/.well-known/ucp` | Which commerce capabilities a merchant offers agents | Universal Commerce Protocol (UCP Tech Council) | 6370 | 3.97% | 3.5–4.5 | new |
| `/.well-known/gpc.json` | Whether the site honors the data-sharing opt-out | W3C Global Privacy Control | 6742 | 2.85% | 2.5–3.3 | → |
| `/security.txt` | Where to report a vulnerability, at the site root | IETF | 6981 | 1.25% | 1.0–1.5 | → |
| `/.well-known/traffic-advice` | Whether a caching proxy may prefetch pages | Google (Private Prefetch Proxy) | 6705 | 1.00% | 0.8–1.3 | → |
| `/rsl.xml` | The license terms under which content may be used | RSL Collective | 6294 | 0.67% | 0.5–0.9 | → |
| `/.well-known/tdmrep.json` | Whether text and data may be mined automatically | W3C TDM Reservation Protocol CG | 6746 | 0.44% | 0.3–0.6 | → |
| `/.well-known/openid-configuration` | Where and how to sign in at this domain | OpenID Foundation | 6715 | 0.40% | 0.3–0.6 | → |
| `/.well-known/api-catalog` | An index of the interfaces a domain offers | IETF | 6722 | 0.27% | 0.2–0.4 | → |
| `/ai.txt` | Which content is withheld from AI training | Spawning | 6567 | 0.24% | 0.2–0.4 | → |
| `/.well-known/agent-skills/index.json` | Which agent skills a domain offers, with version and digest | Cloudflare (Agent Skills Discovery RFC) | 6364 | 0.19% | 0.1–0.3 | new |
| `/.well-known/mcp/server-card.json` | Self-description of a site's MCP server for clients | no registered publisher — singular variant of MCP SEP-2127, checked by Cloudflare's Agent Readiness Score | 6365 | 0.19% | 0.1–0.3 | new |
| `/openapi.json` | A description of an interface for other programs | OpenAPI Initiative | 6299 | 0.17% | 0.1–0.3 | → |
| `/.well-known/ai-catalog.json` | What content and services a domain offers AI agents | AI Catalog WG (Linux Foundation), Google, Microsoft | 6672 | 0.13% | 0.1–0.3 | → |
| `/.well-known/ai-plugin.json` | Instructions for a chatbot to operate a service | OpenAI | 6506 | 0.09% | 0.0–0.2 | → |
| `/.well-known/mcp.json` | Which tool servers a domain provides for AI | Model Context Protocol | 6663 | 0.08% | 0.0–0.2 | → |
| `/.well-known/agent-card.json` | What a software agent can do and how to address it | A2A Project (Linux Foundation) | 6673 | 0.06% | 0.0–0.2 | → |
| `/.well-known/ai.txt` | The same AI usage rules in the well-known folder | Spawning | 6543 | 0.05% | 0.0–0.1 | → |
| `/.well-known/host-meta` | Pointers to a domain's other points of information | IETF | 6711 | 0.04% | 0.0–0.1 | → |
| `/.well-known/did.json` | A domain's provable identity without a central party | W3C | 6647 | 0.03% | 0.0–0.1 | → |
| `/.well-known/dnt-policy.txt` | A pledge not to track visitors across sites | EFF | 6739 | 0.03% | 0.0–0.1 | → |
| `/swagger.json` | An interface description under the older file name | SmartBear (Swagger) | 6226 | 0.03% | 0.0–0.1 | → |
| `/.well-known/agent.json` | An agent's capabilities, under the older file name | A2A Project (Linux Foundation) | 6665 | 0.02% | 0.0–0.1 | → |
| `/.well-known/llms.txt` | A table of contents for language models, in well-known | Answer.AI | 6510 | 0.02% | 0.0–0.1 | → |
| `/.well-known/webfinger` | Who is behind an address at this domain | IETF | 6561 | 0.02% | 0.0–0.1 | → |
| `/.well-known/mcp-server` | Where to reach a domain's tool server | IETF (individual draft) | 6669 | 0.01% | 0.0–0.1 | → |
| `/.well-known/openapi.json` | An interface description in the well-known folder | OpenAPI Initiative | 6625 | 0.00% | 0.0–0.1 | → |
| `/.well-known/openid-federation` | Which federation a party provably belongs to | OpenID Foundation | 6712 | 0.00% | 0.0–0.1 | → |
| `/.well-known/x402.json` | The price and payment route for machine requests | Coinbase, Cloudflare | 6648 | 0.00% | 0.0–0.1 | → |
| `/ai-plugin.json` | The same chatbot instructions, at the site root | OpenAI | 6255 | 0.00% | 0.0–0.1 | → |
| `/mcp.json` | A machine-readable list of a site's MCP endpoints, at the root | Anthropic et al. (MCP) — root-path variant not specified | 6246 | 0.00% | 0.0–0.1 | → |

Adoption is the share of sources we were actually allowed to inspect that
served the route, with a 95% Wilson interval. Sources that turned us away
(bot wall), forbade the fetch via robots.txt, or could not be reached are
counted and reported separately — but a non-answer is not a "no", so they
are not part of the denominator.
**`n` is the number of hosts on which this route was actually probed. It
differs between routes, so each row has its own denominator and the rows
are not directly comparable with one another.**
An arrow appears only where the intervals no longer overlap with **panel-2026-10**; `→` means the change stays within measurement uncertainty.
Trend arrows compare the 10,000-source panel with the previous month (same list, same ruleset). The quarterly roll-up is shown as a level; its first comparison is the February 2027 roll-up.
`new` means the route is measured since this run — it says nothing about when it first appeared on the web.
Of the 1623 `/llms.txt` files found in the whole monthly run `monat-2026-11-block-c` (panel and block), 524 (32.3%) carry the marks of a generator — a self-declared producer or wording shared with other sites; the producers that name themselves are content-management plugins (largest: yoast seo 113, rank math seo 24, all in one seo 17). The adoption figure above counts files, and that stays right: a file rolled out by a plugin exists and is read. This footnote answers the other question — how much of the number is a decision. It is an indication for this run, not a published rate.
Of the 493 `/llms-full.txt` files found in the whole monthly run `monat-2026-11-block-c` (panel and block), 351 (71.2%) carry the marks of a generator — a self-declared producer or wording shared with other sites. The adoption figure above counts files, and that stays right: a file rolled out by a plugin exists and is read. This footnote answers the other question — how much of the number is a decision. It is an indication for this run, not a published rate.

### Notes on this run

- **Cloudflare's robots.txt entry is back.** On the same 1,000 panel sources (readable robots.txt), the entry Cloudflare inserts into robots.txt stood at **7.8%** in September (55/704, 95% CI 6.1–10.0), **2.0%** in October (14/700, 95% CI 1.2–3.3) and **7.2%** in November (50/695, 95% CI 5.5–9.4). The old form disappeared in mid-September (Cloudflare's change of 15 September); a new form ("# Training crawlers"), seen in single files since mid-September, spread from about late October and in November is again close to the September level (41 of 50 in the new form). Read October → November alone, it would look like a new high; it is a return.
- What the new entry asks: in November, 439 of the 10,000 panel sources carry it. 420 of them name AI training crawlers only (for example GPTBot, ClaudeBot, CCBot, Google-Extended), which leaves AI search and requests made on a user's behalf untouched. 19 also ask AI agents acting for users to stay away (ChatGPT-User, Claude-User, Perplexity-User), 6 also AI search crawlers (OAI-SearchBot, PerplexityBot, Claude-SearchBot). robots.txt is a request, not a technical block; we measure only the robots.txt view, not what a firewall does, and not who chose the setting.
- **Full frame September–November 2026** (all 30,000 sources, each measured once; 25,851 reachable organisations): `/robots.txt` 84.6% (95% CI 84.2–85.1, n 22,968) · `/sitemap.xml` 54.0% (95% CI 53.4–54.7, n 20,515) · `/llms.txt` 14.1% (95% CI 13.6–14.6, n 19,764) · `/.well-known/security.txt` 8.5% (95% CI 8.1–8.9, n 20,503). This is a level, not a trend; its first comparison is the February 2027 roll-up.
- From October 2026 the panel has 10,000 sources (a third of the frame). The earlier 1,000-source panel continues inside it as a subset until December 2026 and is published as its own series (`data/panel1000-YYYY-MM.*`); the two series are never chained.
- Of the 132 panel sources that carried Cloudflare's managed robots.txt block in October, those using the marker form still carry a block in 20 of 21 readable files (95.24%, 95% CI 77.3–99.2); those using the preamble-only form in 106 of 108 (98.15%, 95% CI 93.5–99.5).
- 1 file could not be read in November (0.77% of the pair, against 19.2% across the panel) and 2 hosts were unreachable.
- We give no combined rate: it would hide that one notation changed while the setting stayed.
- Content-Signal lines in robots.txt: 530 of 6,483 panel hosts (8.18%, 7.5–8.9); 454 of them sit inside a provider-managed block, 76 (1.17%, 0.9–1.5) outside it.
- Delivers Markdown when Markdown is preferred: 162 of 6,428 organisations (2.52%, 2.2–2.9).
- Announcing a Markdown version beforehand is rarer: `rel="describedby"` 13, `rel="alternate" type="text/markdown"` 3 (a lower bound — only HTTP Link headers are countable).
- A single request cannot tell whether a server negotiates or always serves Markdown.
- Because our one home-page request prefers Markdown, 162 home pages answered without an HTML head; their link relations are not read.
- TDMRep under ruleset 0.4.0: 30 on the panel under the new rule, 30 under the old one (see the version history in RULESET.md).
- 2 organisations declare a licence in robots.txt (`License:`); 1 of them points to `/rsl.xml`.
- 3 organisations announce llms.txt in robots.txt under a path other than the root; the file belongs at the root, so they are not counted.
- DNS: of 10,000 panel sources, 0 publish a specification-conformant `_agent` record; at most 1 `_mcp` answer is neither a wildcard nor SPF.
- `/.well-known/ai-catalog.json`: in the fixed 1,000-source panel 0 of 676 in October and 0 of 675 in November; in the 10,000-source panel 9 of 6,672 (0.13%). Lighthouse has checked the file since 2026.
- Same panel, in October → in November, only hosts observed in both months (new / gone of paired hosts): `/robots.txt` +112 / −42 (n 7,406) · `/sitemap.xml` +54 / −58 (n 6,638) · `/llms.txt` +60 / −20 (n 6,387) · `/.well-known/oauth-protected-resource` +29 / −24 (n 6,549) · `/.well-known/oauth-authorization-server` +26 / −25 (n 6,554) · `/.well-known/security.txt` +18 / −7 (n 6,641).



## Under observation (23)

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
- `/agents.md` — Shopify (platform default) and the AGENTS.md convention from code repositories. How a site describes itself to AI agents
- `/.well-known/ard.json` — ARD specification v0.91 (ards-project) — successor path of /.well-known/ai-catalog.json. Content and services a domain offers AI agents (ARD)

_Observed routes are not requested in the monthly run. Our discovery runs (see below) and a monthly field probe on 1,000 of the panel sources request them, and count nothing from them for this page. Each entry names its promotion criterion in the lab._

### Requested only by discovery runs (27)

- `/.well-known/api-catalog.json`
- `/.well-known/http-message-signatures-directory`
- `/.well-known/signature-agent-card`
- `/.well-known/sail`
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
- `/llms-small.txt`
- `/llms-ctx.txt`
- `/llms-ctx-full.txt`
- `/trust.txt`
- `/.well-known/trust.txt`
- `/.well-known/agent`
- `/.well-known/ucap`
- `/.well-known/ucap-access`
- `/.well-known/ucap-delegation`
- `/.well-known/aauth-access.json`
- `/.well-known/aauth-resource.json`
- `/.well-known/idmandat.json`
- `/.well-known/agents.json`
<!-- RADAR:END -->
**What we request.** The lists above are the complete list of routes we
request: the measured routes in every monthly run; the routes under
observation only in the monthly field probe on 1,000 panel sources and in the
discovery runs; the routes under “Requested only by discovery runs” only in
those. Three additions: your home page, once, to read its `<link rel>`
announcements (the page itself is discarded); when files on your own domain
point to another file there — a link in your `robots.txt`, say — we may fetch
that referenced file, one request per referenced file and run, under
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

The figures above come from the **10,000-source panel**: since October 2026 a
stratified panel of 10,000 sources — a third of the 30,000-source frame — is
measured every month; the earlier 1,000-source panel continues inside it as its
own series (see the notes below the table). Trend arrows compare the panel with
the previous month; the rule is stated below the table. Every other source of
the frame is measured once in each three-month pass through it. The **14-month
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
block source is visited once per quarter. Block **c** ran in November 2026, which completes the first full pass of the frame (September–November 2026). The
block run's purpose is coverage, not trend.

All series are published in [`data/`](data/): `panel-YYYY-MM.{json,csv}`,
`panel1000-YYYY-MM.{json,csv}` and `monat-YYYY-MM-block-x.{json,csv}`; after the last month of each pass also `quartal-YYYY-qN.{json,csv}`, the full frame with every source counted once (its `parts` name the three runs it is built from). Each file states when it was
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
