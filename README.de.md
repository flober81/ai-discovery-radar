# ai-discovery-radar

[English](README.md) · **Deutsch** · [Italiano](README.it.md)

> **Diese Kennung in Ihren Protokollen gefunden?** Sie können sich mit einer
> einzigen Zeile austragen — siehe [Austragung](#austragung). Kein Konto, kein
> Kontakt, keine Begründung nötig.

Ein Radar der KI-Discovery-Dateien im öffentlichen Web: welche Routen es gibt
(`robots.txt`, `llms.txt`, `ai-catalog.json`, …), wie weit sie verbreitet sind
und ob sie sich überhaupt abrufen lassen. Jeder Ausschlag ist eine Messung,
keine Meinung. Wie oft gemessen wird, steht hier, sobald es Läufe gibt, die
das belegen.

## Das Radar

<!-- RADAR:START -->
_34 Routen im Katalog · noch keine veröffentlichte Messung_

| Route | Zweck | Herausgeber | Verbreitung |
|:--|:--|:--|--:|
| `/robots.txt` | Welche Bereiche automatische Abrufer betreten dürfen | IETF | — |
| `/sitemap.xml` | Verzeichnis aller Adressen, die eine Website anbietet | sitemaps.org | — |
| `/.well-known/security.txt` | Wohin man eine Sicherheitslücke meldet | IETF | — |
| `/security.txt` | Wohin man eine Sicherheitslücke meldet, an der Wurzel | IETF | — |
| `/.well-known/api-catalog` | Verzeichnis der Schnittstellen, die eine Domain anbietet | IETF | — |
| `/.well-known/tdmrep.json` | Ob Texte und Daten automatisch ausgewertet werden dürfen | W3C TDM Reservation Protocol CG | — |
| `/.well-known/gpc.json` | Ob die Seite dem Widerspruch gegen Datenweitergabe folgt | W3C Global Privacy Control | — |
| `/.well-known/dnt-policy.txt` | Zusage, Besucher nicht über Seiten hinweg zu verfolgen | EFF | — |
| `/.well-known/host-meta` | Verweise auf die weiteren Auskunftsstellen einer Domain | IETF | — |
| `/.well-known/webfinger` | Wer hinter einer Adresse an dieser Domain steckt | IETF | — |
| `/.well-known/oauth-protected-resource` | Wo ein Client seine Zugangsberechtigung holt | IETF | — |
| `/.well-known/oauth-authorization-server` | Wie die Stelle arbeitet, die Zugangsrechte vergibt | IETF | — |
| `/.well-known/openid-configuration` | Wo und wie man sich bei dieser Domain anmeldet | OpenID Foundation | — |
| `/.well-known/openid-federation` | Zu welchem Verbund eine Stelle nachweislich gehört | OpenID Foundation | — |
| `/.well-known/traffic-advice` | Ob ein Zwischenspeicher Seiten vorab laden darf | Google (Private Prefetch Proxy) | — |
| `/.well-known/ai-catalog.json` | Was eine Domain KI-Agenten an Inhalten und Diensten bietet | AI Catalog WG (Linux Foundation), Google, Microsoft | — |
| `/.well-known/agent-card.json` | Was ein Software-Agent kann und wie man ihn anspricht | A2A Project (Linux Foundation) | — |
| `/.well-known/agent.json` | Fähigkeiten eines Agenten, unter dem alten Dateinamen | A2A Project (Linux Foundation) | — |
| `/.well-known/mcp.json` | Welche Werkzeug-Server eine Domain für KI bereitstellt | Model Context Protocol | — |
| `/.well-known/mcp-server` | Wo der Werkzeug-Server einer Domain zu erreichen ist | IETF (individual draft) | — |
| `/openapi.json` | Beschreibung einer Schnittstelle für fremde Programme | OpenAPI Initiative | — |
| `/.well-known/openapi.json` | Schnittstellen-Beschreibung im Sammelordner der Domain | OpenAPI Initiative | — |
| `/.well-known/x402.json` | Preis und Bezahlweg für maschinelle Abrufe | Coinbase, Cloudflare | — |
| `/.well-known/did.json` | Nachweisbare Identität einer Domain ohne zentrale Stelle | W3C | — |
| `/llms.txt` | Inhaltsverzeichnis für Sprachmodelle | Answer.AI | — |
| `/llms-full.txt` | Der gesamte Inhalt einer Website in einer einzigen Datei | Answer.AI | — |
| `/ai.txt` | Welche Inhalte für das Training von KI gesperrt sind | Spawning | — |
| `/.well-known/ai.txt` | Dieselben KI-Nutzungsregeln im Sammelordner der Domain | Spawning | — |
| `/swagger.json` | Schnittstellen-Beschreibung unter dem alten Dateinamen | SmartBear (Swagger) | — |
| `/rsl.xml` | Zu welchen Lizenzbedingungen Inhalte genutzt werden dürfen | RSL Collective | — |
| `/humans.txt` | Wer eine Website gemacht hat, für Menschen lesbar | humanstxt.org | — |
| `/.well-known/ai-plugin.json` | Anleitung, damit ein Chatbot einen Dienst bedienen kann | OpenAI | — |
| `/ai-plugin.json` | Dieselbe Anleitung für Chatbots, an der Wurzel | OpenAI | — |
| `/.well-known/llms.txt` | Inhaltsverzeichnis für Sprachmodelle im Sammelordner | Answer.AI | — |

Verbreitungszahlen erscheinen mit dem ersten veröffentlichten Lauf.

<!-- RADAR:END -->
Diese Tabelle ist die vollständige Liste der Routen, die wir regulär abfragen.
Eine Ergänzung: Verweisen Dateien Ihrer eigenen Domain auf eine weitere Datei
dort (etwa ein Link in Ihrer `robots.txt`), rufen wir diese verwiesene Datei
gegebenenfalls einmal ab — höchstens ein solcher Folge-Abruf je Domain und
Lauf, unter denselben `robots.txt`-Regeln. Zusätzlich fragen wir je Domain
drei DNS-Namenseinträge ab (`_agent`, `_mcp`, `_index._agents`) — reine
Namensauflösung, die Ihren Webserver nie berührt.
Eine Route steht in der Tabelle, wenn sie
einen benennbaren Herausgeber hat oder ein dokumentierter Konsument sie liest —
nicht, weil sie irgendwo als Format herumgereicht wird. Der Herausgeber steht
in der Tabelle, damit jede Zeile selbst nachprüfbar ist. Der Zweck sagt, was
die Datei an einem Server tut — er beschreibt sie, er bewertet sie nicht.

## Wie gemessen wird

Die Messung respektiert die `robots.txt`, meldet sich ehrlich mit diesem
Repository als Absender und arbeitet langsam und sparsam. Gemessen werden
ausschließlich öffentliche, für Maschinen bestimmte Konfigurationsdateien —
keine Inhalte.

## Austragung

Keine Rückfragen, keine Begründung nötig. Ein Weg genügt:

1. E-Mail an **florian.f.berger@gmail.com** mit der Domain — dafür brauchen Sie
   kein GitHub-Konto, **oder**
2. ein Issue in diesem Repository mit der Domain, **oder**
3. eine `Disallow`-Regel für unsere Kennung in Ihrer `robots.txt` — das wirkt
   ganz ohne Kontakt.

Ausgetragene Domains werden übersprungen, **bevor** überhaupt eine Anfrage
gestellt wird. Kontakt, Korrekturen und die vollständige Zusage:
[SECURITY.md](SECURITY.md).

## Stichproben-Attribution

Die Domain-Stichprobe wird aus der [Tranco-Liste](https://tranco-list.eu/)
gezogen (Forschungs-Ranking; unser eingefrorener Rahmen verweist auf eine
permanente Tranco-Listen-ID) sowie aus den
[Chrome-UX-Report-Toplisten](https://github.com/zakird/crux-top-lists)
(© Google, [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)).
Tranco selbst bündelt mehrere Quellen, darunter die Majestic Million
(© Majestic, [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/)).

## Lizenz

MIT — siehe [LICENSE](LICENSE).
