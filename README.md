# ai-discovery-radar

**English** · [Deutsch](README.de.md) · [Italiano](README.it.md)

> **Found this in your server logs?** You can opt out in one line — see
> [Opt out](#opt-out) below. No account, no contact, no reason required.
>
> **How often we visit:** about **10,700 sources (domains) per month** — a
> rotating share of the ~30,000-source frame, each of those at most once per
> quarter, plus a small fixed share we re-visit every month, so change from one
> month to the next becomes measurable.

A radar of the AI discovery files on the public web: which routes exist
(`robots.txt`, `llms.txt`, `ai-catalog.json`, …), how widely they are used, and
whether they can be fetched at all. Every blip is a measurement, not an opinion.

## The radar

<!-- RADAR:START -->
_Run **panel-2026-08** · 853 reachable hosts (853 registrable domains) · ruleset 0.3.1_

| Route | Purpose | Publisher | n | Adoption | 95% CI | Trend |
|:--|:--|:--|--:|--:|:--|:-:|
| `/robots.txt` | Which parts of a site automated clients may enter | IETF | 760 | 86.45% | 83.8–88.7 | — |
| `/sitemap.xml` | An index of every address a website offers | sitemaps.org | 680 | 54.56% | 50.8–58.3 | — |
| `/llms.txt` | A table of contents for language models | Answer.AI | 662 | 12.99% | 10.6–15.8 | — |
| `/.well-known/security.txt` | Where to report a security vulnerability | IETF | 681 | 6.75% | 5.1–8.9 | — |
| `/.well-known/oauth-authorization-server` | How the service that grants access rights works | IETF | 675 | 5.19% | 3.8–7.1 | — |
| `/llms-full.txt` | A whole website's content in a single file | Answer.AI | 665 | 4.66% | 3.3–6.5 | — |
| `/.well-known/oauth-protected-resource` | Where a client obtains authorization for access | IETF | 676 | 4.59% | 3.2–6.4 | — |
| `/.well-known/gpc.json` | Whether the site honors the data-sharing opt-out | W3C Global Privacy Control | 677 | 2.81% | 1.8–4.3 | — |
| `/humans.txt` | Who built a website, written for people to read | humanstxt.org | 662 | 1.66% | 0.9–3.0 | — |
| `/.well-known/traffic-advice` | Whether a caching proxy may prefetch pages | Google (Private Prefetch Proxy) | 673 | 1.34% | 0.7–2.5 | — |
| `/security.txt` | Where to report a vulnerability, at the site root | IETF | 696 | 1.15% | 0.6–2.3 | — |
| `/rsl.xml` | The license terms under which content may be used | RSL Collective | 640 | 0.78% | 0.3–1.8 | — |
| `/ai.txt` | Which content is withheld from AI training | Spawning | 667 | 0.45% | 0.2–1.3 | — |
| `/.well-known/tdmrep.json` | Whether text and data may be mined automatically | W3C TDM Reservation Protocol CG | 678 | 0.29% | 0.1–1.1 | — |
| `/.well-known/api-catalog` | An index of the interfaces a domain offers | IETF | 678 | 0.15% | 0.0–0.8 | — |
| `/.well-known/mcp.json` | Which tool servers a domain provides for AI | Model Context Protocol | 674 | 0.15% | 0.0–0.8 | — |
| `/.well-known/openid-configuration` | Where and how to sign in at this domain | OpenID Foundation | 674 | 0.15% | 0.0–0.8 | — |
| `/openapi.json` | A description of an interface for other programs | OpenAPI Initiative | 650 | 0.15% | 0.0–0.9 | — |
| `/.well-known/agent-card.json` | What a software agent can do and how to address it | A2A Project (Linux Foundation) | 672 | 0.00% | 0.0–0.6 | — |
| `/.well-known/agent.json` | An agent's capabilities, under the older file name | A2A Project (Linux Foundation) | 672 | 0.00% | 0.0–0.6 | — |
| `/.well-known/ai-catalog.json` | What content and services a domain offers AI agents | AI Catalog WG (Linux Foundation), Google, Microsoft | 671 | 0.00% | 0.0–0.6 | — |
| `/.well-known/ai-plugin.json` | Instructions for a chatbot to operate a service | OpenAI | 656 | 0.00% | 0.0–0.6 | — |
| `/.well-known/ai.txt` | The same AI usage rules in the well-known folder | Spawning | 661 | 0.00% | 0.0–0.6 | — |
| `/.well-known/did.json` | A domain's provable identity without a central party | W3C | 672 | 0.00% | 0.0–0.6 | — |
| `/.well-known/dnt-policy.txt` | A pledge not to track visitors across sites | EFF | 678 | 0.00% | 0.0–0.6 | — |
| `/.well-known/host-meta` | Pointers to a domain's other points of information | IETF | 670 | 0.00% | 0.0–0.6 | — |
| `/.well-known/llms.txt` | A table of contents for language models, in well-known | Answer.AI | 658 | 0.00% | 0.0–0.6 | — |
| `/.well-known/mcp-server` | Where to reach a domain's tool server | IETF (individual draft) | 673 | 0.00% | 0.0–0.6 | — |
| `/.well-known/openapi.json` | An interface description in the well-known folder | OpenAPI Initiative | 673 | 0.00% | 0.0–0.6 | — |
| `/.well-known/openid-federation` | Which federation a party provably belongs to | OpenID Foundation | 677 | 0.00% | 0.0–0.6 | — |
| `/.well-known/webfinger` | Who is behind an address at this domain | IETF | 671 | 0.00% | 0.0–0.6 | — |
| `/.well-known/x402.json` | The price and payment route for machine requests | Coinbase, Cloudflare | 670 | 0.00% | 0.0–0.6 | — |
| `/ai-plugin.json` | The same chatbot instructions, at the site root | OpenAI | 641 | 0.00% | 0.0–0.6 | — |
| `/swagger.json` | An interface description under the older file name | SmartBear (Swagger) | 642 | 0.00% | 0.0–0.6 | — |

Adoption is the share of sources we were actually allowed to inspect that
served the route, with a 95% Wilson interval. Sources that turned us away
(bot wall), forbade the fetch via robots.txt, or could not be reached are
counted and reported separately — but a non-answer is not a "no", so they
are not part of the denominator.
**`n` is the number of hosts on which this route was actually probed. It
differs between routes, so each row has its own denominator and the rows
are not directly comparable with one another.**
No previous run to compare against yet.



## Under observation (18)

**Confirmed** — registered (IANA) or RFC, barely seen in the field yet:

- `/.well-known/nostr.json` — Nostr Developer Community (NIP-05). Proof that a public key belongs to a name at this domain
- `/.well-known/vacation-rental.json` — Vacation Rental Protocol (Einzelregistrant). Discovery document for cryptographically signed stay offers
- `/.well-known/xregistry` — xRegistry Authors (CNCF Sandbox). Entry point of an extensible registry for schemas and events
- `/.well-known/host-meta.json` — IETF. JSON twin of the host-meta pointers

**Emerging** — field signals or drafts, no registration yet:

- `/.well-known/atproto-did` — AT Protocol (Bluesky). Resolves a domain handle to a decentralized identity
- `/server-card.json` — kursierende Agenten-Spec ohne benennbaren Herausgeber. A proposed self-description card for agent-facing servers
- `/product.xml` — kein Herausgeber — Commerce-Konvention im Entstehen. Product listings that shops link for machine readers
- `Signposting (Link-Header: describedby/cite-as/linkset)` — FAIR Signposting Profile (Wissenschafts-Repositorien-Community). Machine-readable pointers from scholarly pages to their metadata and full texts
- `/.well-known/jwt-vc-issuer` — IETF (OAuth-Arbeitsgruppe, Entwurfsstadium). Where a verifier finds an issuer's keys for verifiable credentials
- `/.well-known/ai` — IETF-Entwurf (AI Discovery Endpoint). A proposed machine-readable capability description for AI agents
- `_agent (DNS-TXT, keine HTTP-Route)` — IETF-Entwurf (Agent Identity and Discovery, AID). A DNS record proposing agent identity discovery
- `Content-Usage (robots-Direktive + HTTP-Header, kein Pfad)` — IETF-AIPREF-Arbeitsgruppe (draft-ietf-aipref-attach, WG-adopted, Standards-Track). A directive stating what AI may do with the content
- `Schemamap (robots-Direktive; Ziel-URL frei, konventionell auch /schema.txt)` — SCHEMA.TXT (Spezifikation auf GitHub) — ausgerollt u. a. durch Yoast (Schema-Aggregator-Endpunkt). A directive pointing machines to a site's schema map
- `/.well-known/did-configuration.json` — Decentralized Identity Foundation (DIF). Proof linking a domain to decentralized identifiers
- `_apertoid (DNS-TXT, keine HTTP-Route)` — ApertoID (Einzelanbieter). A DNS record for an emerging open-identity proposal
- `_x402 (DNS-TXT) + /.well-known/x402` — Individual-Draft (W. Hawkins) zum Coinbase/Cloudflare-x402. DNS and web discovery of x402 payment endpoints
- `_agents / AIDISCA+AIINDEX (neue DNS-RR-Typen)` — Verisign (Individual-Draft, institutionell gewichtig). Proposed DNS record types for agent discovery
- `Link rel=client-ranges (HTTP-Link-Header)` — Individual-Draft (Google-/Ericsson-Autoren). A header pointing clients to declared IP ranges

_Observed means observed — none of these are measured or counted above. Each entry names its promotion criterion in the lab._
<!-- RADAR:END -->
**What we request.** The table above is the complete list of routes we
routinely request. Two additions: when files on your own domain point to
another file there — a link in your `robots.txt`, say — we may fetch that
referenced file once, at most one such follow-up per domain and run, under the
same `robots.txt` rules. And we look up three DNS records per domain
(`_agent`, `_mcp`, `_index._agents`): plain name-service lookups that never
touch your web server.

**How a route gets into the table.** It needs a nameable publisher or a
documented consumer that reads it — not merely a format being passed around
somewhere. The publisher is in the table so that every row can be checked on
its own. The purpose says what the file does on a server; it describes the
file, it does not judge it.

## How we measure

The measurement obeys your `robots.txt`, identifies itself honestly with this
repository as the sender, and works slowly and sparingly. Only public
configuration files meant for machines are fetched — no page content.

The figures above are the **August 2026 baseline**: a stratified panel of
1,000 sources, measured once. From **September 2026** the panel is measured
monthly, and every source in the wider sample once per quarter. Alongside the
first monthly report, a **14-month review** of AI directive adoption
(June 2025 – July 2026) will be published, based on more than **270,000
evaluated robots.txt files**.

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
3. put a `Disallow` rule for our token in your `robots.txt` — this works without
   contacting us at all.

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
