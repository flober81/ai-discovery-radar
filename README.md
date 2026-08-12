# ai-discovery-radar

**English** · [Deutsch](README.de.md) · [Italiano](README.it.md)

> **Found this in your server logs?** You can opt out in one line — see
> [Opt out](#opt-out) below. No account, no contact, no reason required.

A radar of the AI discovery files on the public web: which routes exist
(`robots.txt`, `llms.txt`, `ai-catalog.json`, …), how widely they are used, and
whether they can be fetched at all. Every blip is a measurement, not an opinion.
How often we measure will be stated here once there are runs to back it up.

## The radar

<!-- RADAR:START -->
_34 routes in the catalog · no published measurement yet_

| Route | Purpose | Publisher | Adoption |
|:--|:--|:--|--:|
| `/robots.txt` | Which parts of a site automated clients may enter | IETF | — |
| `/sitemap.xml` | An index of every address a website offers | sitemaps.org | — |
| `/.well-known/security.txt` | Where to report a security vulnerability | IETF | — |
| `/security.txt` | Where to report a vulnerability, at the site root | IETF | — |
| `/.well-known/api-catalog` | An index of the interfaces a domain offers | IETF | — |
| `/.well-known/tdmrep.json` | Whether text and data may be mined automatically | W3C TDM Reservation Protocol CG | — |
| `/.well-known/gpc.json` | Whether the site honors the data-sharing opt-out | W3C Global Privacy Control | — |
| `/.well-known/dnt-policy.txt` | A pledge not to track visitors across sites | EFF | — |
| `/.well-known/host-meta` | Pointers to a domain's other points of information | IETF | — |
| `/.well-known/webfinger` | Who is behind an address at this domain | IETF | — |
| `/.well-known/oauth-protected-resource` | Where a client obtains authorization for access | IETF | — |
| `/.well-known/oauth-authorization-server` | How the service that grants access rights works | IETF | — |
| `/.well-known/openid-configuration` | Where and how to sign in at this domain | OpenID Foundation | — |
| `/.well-known/openid-federation` | Which federation a party provably belongs to | OpenID Foundation | — |
| `/.well-known/traffic-advice` | Whether a caching proxy may prefetch pages | Google (Private Prefetch Proxy) | — |
| `/.well-known/ai-catalog.json` | What content and services a domain offers AI agents | AI Catalog WG (Linux Foundation), Google, Microsoft | — |
| `/.well-known/agent-card.json` | What a software agent can do and how to address it | A2A Project (Linux Foundation) | — |
| `/.well-known/agent.json` | An agent's capabilities, under the older file name | A2A Project (Linux Foundation) | — |
| `/.well-known/mcp.json` | Which tool servers a domain provides for AI | Model Context Protocol | — |
| `/.well-known/mcp-server` | Where to reach a domain's tool server | IETF (individual draft) | — |
| `/openapi.json` | A description of an interface for other programs | OpenAPI Initiative | — |
| `/.well-known/openapi.json` | An interface description in the well-known folder | OpenAPI Initiative | — |
| `/.well-known/x402.json` | The price and payment route for machine requests | Coinbase, Cloudflare | — |
| `/.well-known/did.json` | A domain's provable identity without a central party | W3C | — |
| `/llms.txt` | A table of contents for language models | Answer.AI | — |
| `/llms-full.txt` | A whole website's content in a single file | Answer.AI | — |
| `/ai.txt` | Which content is withheld from AI training | Spawning | — |
| `/.well-known/ai.txt` | The same AI usage rules in the well-known folder | Spawning | — |
| `/swagger.json` | An interface description under the older file name | SmartBear (Swagger) | — |
| `/rsl.xml` | The license terms under which content may be used | RSL Collective | — |
| `/humans.txt` | Who built a website, written for people to read | humanstxt.org | — |
| `/.well-known/ai-plugin.json` | Instructions for a chatbot to operate a service | OpenAI | — |
| `/ai-plugin.json` | The same chatbot instructions, at the site root | OpenAI | — |
| `/.well-known/llms.txt` | A table of contents for language models, in well-known | Answer.AI | — |

Adoption figures will appear with the first published run.

<!-- RADAR:END -->
This table is complete: it lists every route we request, and whatever is not in
it, we do not request. A route is listed when it has a nameable publisher or a
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

The domain sample comes from the Majestic Million
(© Majestic, [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/)).

## License

MIT — see [LICENSE](LICENSE).
