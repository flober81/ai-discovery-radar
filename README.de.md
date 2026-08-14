# ai-discovery-radar

[English](README.md) · **Deutsch** · [Italiano](README.it.md)

> **Diese Kennung in Ihren Protokollen gefunden?** Sie können sich mit einer
> einzigen Zeile austragen — siehe [Austragung](#austragung). Kein Konto, kein
> Kontakt, keine Begründung nötig.

Ein Radar der KI-Discovery-Dateien im öffentlichen Web: welche Routen es gibt
(`robots.txt`, `llms.txt`, `ai-catalog.json`, …), wie weit sie verbreitet sind
und ob sie sich überhaupt abrufen lassen. Jeder Ausschlag ist eine Messung,
keine Meinung. Die Tabelle unten zeigt die **August-2026-Basislinie**: ein
geschichtetes Panel von 1.000 Domains, einmal gemessen. Ab **September 2026**
wird das Panel monatlich gemessen, jede Domain der größeren Stichprobe einmal
pro Quartal.

## Das Radar

<!-- RADAR:START -->
_Lauf **panel-2026-08** · 853 erreichbare Hosts (853 registrierbare Domains) · Regelsatz 0.2.0_

| Route | Zweck | Herausgeber | n | Verbreitung | 95 % KI | Trend |
|:--|:--|:--|--:|--:|:--|:-:|
| `/robots.txt` | Welche Bereiche automatische Abrufer betreten dürfen | IETF | 853 | 77,02 % | 74,1–79,7 | — |
| `/sitemap.xml` | Verzeichnis aller Adressen, die eine Website anbietet | sitemaps.org | 842 | 44,06 % | 40,7–47,4 | — |
| `/llms.txt` | Inhaltsverzeichnis für Sprachmodelle | Answer.AI | 842 | 10,21 % | 8,3–12,4 | — |
| `/.well-known/security.txt` | Wohin man eine Sicherheitslücke meldet | IETF | 842 | 5,46 % | 4,1–7,2 | — |
| `/.well-known/oauth-authorization-server` | Wie die Stelle arbeitet, die Zugangsrechte vergibt | IETF | 842 | 4,16 % | 3,0–5,7 | — |
| `/.well-known/oauth-protected-resource` | Wo ein Client seine Zugangsberechtigung holt | IETF | 842 | 3,68 % | 2,6–5,2 | — |
| `/llms-full.txt` | Der gesamte Inhalt einer Website in einer einzigen Datei | Answer.AI | 842 | 3,68 % | 2,6–5,2 | — |
| `/.well-known/gpc.json` | Ob die Seite dem Widerspruch gegen Datenweitergabe folgt | W3C Global Privacy Control | 842 | 2,26 % | 1,4–3,5 | — |
| `/humans.txt` | Wer eine Website gemacht hat, für Menschen lesbar | humanstxt.org | 842 | 1,31 % | 0,7–2,3 | — |
| `/.well-known/traffic-advice` | Ob ein Zwischenspeicher Seiten vorab laden darf | Google (Private Prefetch Proxy) | 842 | 1,07 % | 0,6–2,0 | — |
| `/security.txt` | Wohin man eine Sicherheitslücke meldet, an der Wurzel | IETF | 842 | 0,95 % | 0,5–1,9 | — |
| `/rsl.xml` | Zu welchen Lizenzbedingungen Inhalte genutzt werden dürfen | RSL Collective | 842 | 0,59 % | 0,3–1,4 | — |
| `/ai.txt` | Welche Inhalte für das Training von KI gesperrt sind | Spawning | 842 | 0,36 % | 0,1–1,0 | — |
| `/.well-known/tdmrep.json` | Ob Texte und Daten automatisch ausgewertet werden dürfen | W3C TDM Reservation Protocol CG | 842 | 0,24 % | 0,1–0,9 | — |
| `/.well-known/api-catalog` | Verzeichnis der Schnittstellen, die eine Domain anbietet | IETF | 842 | 0,12 % | 0,0–0,7 | — |
| `/.well-known/mcp.json` | Welche Werkzeug-Server eine Domain für KI bereitstellt | Model Context Protocol | 842 | 0,12 % | 0,0–0,7 | — |
| `/.well-known/openid-configuration` | Wo und wie man sich bei dieser Domain anmeldet | OpenID Foundation | 842 | 0,12 % | 0,0–0,7 | — |
| `/openapi.json` | Beschreibung einer Schnittstelle für fremde Programme | OpenAPI Initiative | 842 | 0,12 % | 0,0–0,7 | — |
| `/.well-known/agent-card.json` | Was ein Software-Agent kann und wie man ihn anspricht | A2A Project (Linux Foundation) | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/agent.json` | Fähigkeiten eines Agenten, unter dem alten Dateinamen | A2A Project (Linux Foundation) | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/ai-catalog.json` | Was eine Domain KI-Agenten an Inhalten und Diensten bietet | AI Catalog WG (Linux Foundation), Google, Microsoft | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/ai-plugin.json` | Anleitung, damit ein Chatbot einen Dienst bedienen kann | OpenAI | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/ai.txt` | Dieselben KI-Nutzungsregeln im Sammelordner der Domain | Spawning | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/did.json` | Nachweisbare Identität einer Domain ohne zentrale Stelle | W3C | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/dnt-policy.txt` | Zusage, Besucher nicht über Seiten hinweg zu verfolgen | EFF | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/host-meta` | Verweise auf die weiteren Auskunftsstellen einer Domain | IETF | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/llms.txt` | Inhaltsverzeichnis für Sprachmodelle im Sammelordner | Answer.AI | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/mcp-server` | Wo der Werkzeug-Server einer Domain zu erreichen ist | IETF (individual draft) | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/openapi.json` | Schnittstellen-Beschreibung im Sammelordner der Domain | OpenAPI Initiative | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/openid-federation` | Zu welchem Verbund eine Stelle nachweislich gehört | OpenID Foundation | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/webfinger` | Wer hinter einer Adresse an dieser Domain steckt | IETF | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/x402.json` | Preis und Bezahlweg für maschinelle Abrufe | Coinbase, Cloudflare | 842 | 0,00 % | 0,0–0,5 | — |
| `/ai-plugin.json` | Dieselbe Anleitung für Chatbots, an der Wurzel | OpenAI | 842 | 0,00 % | 0,0–0,5 | — |
| `/swagger.json` | Schnittstellen-Beschreibung unter dem alten Dateinamen | SmartBear (Swagger) | 842 | 0,00 % | 0,0–0,5 | — |

Verbreitung ist der Anteil erreichbarer Hosts, die die Route ausgeliefert haben,
mit einem 95-%-Wilson-Intervall. Jede Zahl ist eine Untergrenze aus Sicht eines
nicht privilegierten Agenten: Eine Datei, die existiert, aber nicht abgerufen
werden darf, zählt nicht mit.
**`n` ist die Anzahl der Hosts, auf denen diese Route tatsächlich geprobt
wurde — sie unterscheidet sich zwischen den Routen, daher hat jede Zeile
ihren eigenen Nenner und die Zeilen sind nicht direkt miteinander
vergleichbar.**
Noch kein Vorlauf zum Vergleich vorhanden.

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
