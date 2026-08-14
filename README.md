# ai-discovery-radar

**English** · [Deutsch](README.de.md) · [Italiano](README.it.md)

> **Found this in your server logs?** You can opt out in one line — see
> [Opt out](#opt-out) below. No account, no contact, no reason required.

A radar of the AI discovery files on the public web: which routes exist
(`robots.txt`, `llms.txt`, `ai-catalog.json`, …), how widely they are used, and
whether they can be fetched at all. Every blip is a measurement, not an opinion.
The table below shows the **August 2026 baseline**: a stratified panel of
1,000 domains, measured once. From **September 2026** the panel is measured
monthly, and every domain in the wider sample once per quarter.

## The radar

<!-- RADAR:START -->
_Run **panel-2026-08** · 853 reachable hosts (853 registrable domains) · ruleset 0.2.0_

| Route | Purpose | Publisher | n | Adoption | 95% CI | Trend |
|:--|:--|:--|--:|--:|:--|:-:|
| `/robots.txt` | Which parts of a site automated clients may enter | IETF | 853 | 77.02% | 74.1–79.7 | — |
| `/sitemap.xml` | An index of every address a website offers | sitemaps.org | 842 | 44.06% | 40.7–47.4 | — |
| `/llms.txt` | A table of contents for language models | Answer.AI | 842 | 10.21% | 8.3–12.4 | — |
| `/.well-known/security.txt` | Where to report a security vulnerability | IETF | 842 | 5.46% | 4.1–7.2 | — |
| `/.well-known/oauth-authorization-server` | How the service that grants access rights works | IETF | 842 | 4.16% | 3.0–5.7 | — |
| `/.well-known/oauth-protected-resource` | Where a client obtains authorization for access | IETF | 842 | 3.68% | 2.6–5.2 | — |
| `/llms-full.txt` | A whole website's content in a single file | Answer.AI | 842 | 3.68% | 2.6–5.2 | — |
| `/.well-known/gpc.json` | Whether the site honors the data-sharing opt-out | W3C Global Privacy Control | 842 | 2.26% | 1.4–3.5 | — |
| `/humans.txt` | Who built a website, written for people to read | humanstxt.org | 842 | 1.31% | 0.7–2.3 | — |
| `/.well-known/traffic-advice` | Whether a caching proxy may prefetch pages | Google (Private Prefetch Proxy) | 842 | 1.07% | 0.6–2.0 | — |
| `/security.txt` | Where to report a vulnerability, at the site root | IETF | 842 | 0.95% | 0.5–1.9 | — |
| `/rsl.xml` | The license terms under which content may be used | RSL Collective | 842 | 0.59% | 0.3–1.4 | — |
| `/ai.txt` | Which content is withheld from AI training | Spawning | 842 | 0.36% | 0.1–1.0 | — |
| `/.well-known/tdmrep.json` | Whether text and data may be mined automatically | W3C TDM Reservation Protocol CG | 842 | 0.24% | 0.1–0.9 | — |
| `/.well-known/api-catalog` | An index of the interfaces a domain offers | IETF | 842 | 0.12% | 0.0–0.7 | — |
| `/.well-known/mcp.json` | Which tool servers a domain provides for AI | Model Context Protocol | 842 | 0.12% | 0.0–0.7 | — |
| `/.well-known/openid-configuration` | Where and how to sign in at this domain | OpenID Foundation | 842 | 0.12% | 0.0–0.7 | — |
| `/openapi.json` | A description of an interface for other programs | OpenAPI Initiative | 842 | 0.12% | 0.0–0.7 | — |
| `/.well-known/agent-card.json` | What a software agent can do and how to address it | A2A Project (Linux Foundation) | 842 | 0.00% | 0.0–0.5 | — |
| `/.well-known/agent.json` | An agent's capabilities, under the older file name | A2A Project (Linux Foundation) | 842 | 0.00% | 0.0–0.5 | — |
| `/.well-known/ai-catalog.json` | What content and services a domain offers AI agents | AI Catalog WG (Linux Foundation), Google, Microsoft | 842 | 0.00% | 0.0–0.5 | — |
| `/.well-known/ai-plugin.json` | Instructions for a chatbot to operate a service | OpenAI | 842 | 0.00% | 0.0–0.5 | — |
| `/.well-known/ai.txt` | The same AI usage rules in the well-known folder | Spawning | 842 | 0.00% | 0.0–0.5 | — |
| `/.well-known/did.json` | A domain's provable identity without a central party | W3C | 842 | 0.00% | 0.0–0.5 | — |
| `/.well-known/dnt-policy.txt` | A pledge not to track visitors across sites | EFF | 842 | 0.00% | 0.0–0.5 | — |
| `/.well-known/host-meta` | Pointers to a domain's other points of information | IETF | 842 | 0.00% | 0.0–0.5 | — |
| `/.well-known/llms.txt` | A table of contents for language models, in well-known | Answer.AI | 842 | 0.00% | 0.0–0.5 | — |
| `/.well-known/mcp-server` | Where to reach a domain's tool server | IETF (individual draft) | 842 | 0.00% | 0.0–0.5 | — |
| `/.well-known/openapi.json` | An interface description in the well-known folder | OpenAPI Initiative | 842 | 0.00% | 0.0–0.5 | — |
| `/.well-known/openid-federation` | Which federation a party provably belongs to | OpenID Foundation | 842 | 0.00% | 0.0–0.5 | — |
| `/.well-known/webfinger` | Who is behind an address at this domain | IETF | 842 | 0.00% | 0.0–0.5 | — |
| `/.well-known/x402.json` | The price and payment route for machine requests | Coinbase, Cloudflare | 842 | 0.00% | 0.0–0.5 | — |
| `/ai-plugin.json` | The same chatbot instructions, at the site root | OpenAI | 842 | 0.00% | 0.0–0.5 | — |
| `/swagger.json` | An interface description under the older file name | SmartBear (Swagger) | 842 | 0.00% | 0.0–0.5 | — |

Adoption is the share of reachable hosts that served the route, with a
95% Wilson interval. Every figure is a lower bound as seen by an
unprivileged agent: a file that exists but may not be fetched does not
count.
**`n` is the number of hosts on which this route was actually probed. It
differs between routes, so each row has its own denominator and the rows
are not directly comparable with one another.**
No previous run to compare against yet.

<!-- RADAR:END -->
This table is the complete list of routes we routinely request. One addition:
when files on your own domain point to another file there (for example a link
in your `robots.txt`), we may fetch that referenced file once — at most one
such follow-up per domain and run, under the same `robots.txt` rules. We also
look up three DNS records per domain (`_agent`, `_mcp`, `_index._agents`) —
plain name-service lookups that never touch your web server.
A route is listed when it has a nameable publisher or a
documented consumer that reads it — not because some format is being passed
around somewhere. The publisher is in the table so that every row can be checked
on its own. The purpose says what the file does on a server; it describes the
file, it does not judge it.

## How we measure

The measurement obeys your `robots.txt`, identifies itself honestly with this
repository as the sender, and works slowly and sparingly. Only public
configuration files meant for machines are fetched — no page content.

## Opt out

No questions asked, no reason needed. Any one of these is enough:

1. Email **florian.f.berger@gmail.com** with the domain — you do not need a
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
