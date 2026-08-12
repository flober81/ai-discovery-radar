# ai-discovery-radar

> This project is documented in German. It measures the adoption of public
> AI-discovery files (`robots.txt`, `llms.txt`, …).
> **Opt out:** open an issue with your domain or email florian.f.berger@gmail.com
> — no reason required.

Ein regelmäßig gemessenes Radar der KI-Discovery-Dateien im öffentlichen
Web — welche Routen es gibt (`robots.txt`, `llms.txt`, `ai-catalog.json`, …),
wie weit sie verbreitet sind und ob sie sich überhaupt abrufen lassen.
Jeder Ausschlag ist eine Messung, keine Meinung.

## Radar

<!-- RADAR:START -->
_40 Routen im Katalog · noch keine veröffentlichte Messung_

| Route | Herausgeber | Verbreitung |
|:--|:--|--:|
| `/robots.txt` | IETF | — |
| `/sitemap.xml` | sitemaps.org | — |
| `/.well-known/security.txt` | IETF | — |
| `/security.txt` | IETF | — |
| `/.well-known/api-catalog` | IETF | — |
| `/.well-known/tdmrep.json` | W3C TDM Reservation Protocol CG | — |
| `/.well-known/gpc.json` | W3C Global Privacy Control | — |
| `/.well-known/dnt-policy.txt` | EFF | — |
| `/.well-known/nodeinfo` | NodeInfo Community | — |
| `/.well-known/host-meta` | IETF | — |
| `/.well-known/webfinger` | IETF | — |
| `/.well-known/oauth-protected-resource` | IETF | — |
| `/.well-known/oauth-authorization-server` | IETF | — |
| `/.well-known/openid-configuration` | OpenID Foundation | — |
| `/.well-known/openid-federation` | OpenID Foundation | — |
| `/.well-known/traffic-advice` | Google (Private Prefetch Proxy) | — |
| `/.well-known/assetlinks.json` | Google (Digital Asset Links) · Vergleichsgröße | — |
| `/.well-known/change-password` | W3C Web Application Security WG · Vergleichsgröße | — |
| `/.well-known/ai-catalog.json` | AI Catalog WG (Linux Foundation), Google, Microsoft | — |
| `/.well-known/agent-card.json` | A2A Project (Linux Foundation) | — |
| `/.well-known/agent.json` | A2A Project (Linux Foundation) | — |
| `/.well-known/mcp.json` | Model Context Protocol | — |
| `/.well-known/mcp-server` | IETF-Entwurf (MCP-Discovery) | — |
| `/openapi.json` | OpenAPI Initiative | — |
| `/.well-known/openapi.json` | OpenAPI Initiative | — |
| `/.well-known/x402.json` | Coinbase, Cloudflare | — |
| `/.well-known/did.json` | W3C | — |
| `/llms.txt` | Answer.AI | — |
| `/llms-full.txt` | Answer.AI | — |
| `/ai.txt` | Spawning | — |
| `/.well-known/ai.txt` | Platzierungsvariante von /ai.txt | — |
| `/swagger.json` | SmartBear (Swagger) | — |
| `/rsl.xml` | RSL Collective | — |
| `/humans.txt` | humanstxt.org | — |
| `/ads.txt` | IAB Tech Lab · Vergleichsgröße | — |
| `/app-ads.txt` | IAB Tech Lab · Vergleichsgröße | — |
| `/.well-known/apple-app-site-association` | Apple · Vergleichsgröße | — |
| `/.well-known/ai-plugin.json` | OpenAI | — |
| `/ai-plugin.json` | OpenAI | — |
| `/.well-known/llms.txt` | Platzierungsvariante von /llms.txt | — |

Verbreitungszahlen erscheinen mit dem ersten veröffentlichten Lauf.

Als **Vergleichsgröße** gekennzeichnete Routen sind keine KI-Discovery-Routen.
Sie werden mitgemessen, weil sie zeigen, wie Verbreitung aussieht, wenn ein
maschinenlesbares Format seit Jahren durchgesetzt ist. Ohne diesen Maßstab lässt
sich eine kleine Zahl bei einem jungen Format nicht einordnen.

<!-- RADAR:END -->
Diese Tabelle ist vollständig: Sie listet jede Route, die abgefragt wird, und
was dort nicht steht, fragen wir nicht ab. Eine Route steht darin, wenn sie
einen benennbaren Herausgeber hat oder ein dokumentierter Konsument sie liest —
nicht, weil sie irgendwo als Format herumgereicht wird. Der Herausgeber steht
in der Tabelle, damit jede Zeile selbst nachprüfbar ist.

## Wie gemessen wird

Die Messung respektiert die `robots.txt`, meldet sich ehrlich mit diesem
Repository als Absender und arbeitet langsam und sparsam. Gemessen werden
ausschließlich öffentliche, für Maschinen bestimmte Konfigurationsdateien —
keine Inhalte.

## Austragung

Siehe [SECURITY.md](SECURITY.md). Ausgetragene Domains werden übersprungen,
bevor überhaupt eine Anfrage gestellt wird.

## Stichproben-Attribution

Die Domain-Stichprobe stammt aus der Majestic Million
(© Majestic, [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/)).

## Lizenz

MIT — siehe [LICENSE](LICENSE).
