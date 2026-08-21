# ai-discovery-radar

[English](README.md) · **Deutsch** · [Italiano](README.it.md)

> **Diese Kennung in Ihren Protokollen gefunden?** Sie können sich mit einer
> einzigen Zeile austragen — siehe [Austragung](#austragung). Kein Konto, kein
> Kontakt, keine Begründung nötig.
>
> **Wie oft wir vorbeikommen:** rund **10.700 Quellen (Domains) pro Monat** —
> ein rotierender Teil des ~30.000er-Rahmens, jede dieser Quellen höchstens
> einmal pro Quartal, dazu ein kleiner fester Teil, den wir jeden Monat erneut
> besuchen, damit Veränderung von Monat zu Monat messbar wird.

Ein Radar der KI-Discovery-Dateien im öffentlichen Web: welche Routen es gibt
(`robots.txt`, `llms.txt`, `ai-catalog.json`, …), wie weit sie verbreitet sind
und ob sie sich überhaupt abrufen lassen. Jeder Ausschlag ist eine Messung,
keine Meinung.

## Das Radar

<!-- RADAR:START -->
_Lauf **panel-2026-08** · 853 erreichbare Hosts (853 registrierbare Domains) · Regelsatz 0.3.1_

| Route | Zweck | Herausgeber | n | Verbreitung | 95 % KI | Trend |
|:--|:--|:--|--:|--:|:--|:-:|
| `/robots.txt` | Welche Bereiche automatische Abrufer betreten dürfen | IETF | 760 | 86,45 % | 83,8–88,7 | — |
| `/sitemap.xml` | Verzeichnis aller Adressen, die eine Website anbietet | sitemaps.org | 680 | 54,56 % | 50,8–58,3 | — |
| `/llms.txt` | Inhaltsverzeichnis für Sprachmodelle | Answer.AI | 662 | 12,99 % | 10,6–15,8 | — |
| `/.well-known/security.txt` | Wohin man eine Sicherheitslücke meldet | IETF | 681 | 6,75 % | 5,1–8,9 | — |
| `/.well-known/oauth-authorization-server` | Wie die Stelle arbeitet, die Zugangsrechte vergibt | IETF | 675 | 5,19 % | 3,8–7,1 | — |
| `/llms-full.txt` | Der gesamte Inhalt einer Website in einer einzigen Datei | Answer.AI | 665 | 4,66 % | 3,3–6,5 | — |
| `/.well-known/oauth-protected-resource` | Wo ein Client seine Zugangsberechtigung holt | IETF | 676 | 4,59 % | 3,2–6,4 | — |
| `/.well-known/gpc.json` | Ob die Seite dem Widerspruch gegen Datenweitergabe folgt | W3C Global Privacy Control | 677 | 2,81 % | 1,8–4,3 | — |
| `/humans.txt` | Wer eine Website gemacht hat, für Menschen lesbar | humanstxt.org | 662 | 1,66 % | 0,9–3,0 | — |
| `/.well-known/traffic-advice` | Ob ein Zwischenspeicher Seiten vorab laden darf | Google (Private Prefetch Proxy) | 673 | 1,34 % | 0,7–2,5 | — |
| `/security.txt` | Wohin man eine Sicherheitslücke meldet, an der Wurzel | IETF | 696 | 1,15 % | 0,6–2,3 | — |
| `/rsl.xml` | Zu welchen Lizenzbedingungen Inhalte genutzt werden dürfen | RSL Collective | 640 | 0,78 % | 0,3–1,8 | — |
| `/ai.txt` | Welche Inhalte für das Training von KI gesperrt sind | Spawning | 667 | 0,45 % | 0,2–1,3 | — |
| `/.well-known/tdmrep.json` | Ob Texte und Daten automatisch ausgewertet werden dürfen | W3C TDM Reservation Protocol CG | 678 | 0,29 % | 0,1–1,1 | — |
| `/.well-known/api-catalog` | Verzeichnis der Schnittstellen, die eine Domain anbietet | IETF | 678 | 0,15 % | 0,0–0,8 | — |
| `/.well-known/mcp.json` | Welche Werkzeug-Server eine Domain für KI bereitstellt | Model Context Protocol | 674 | 0,15 % | 0,0–0,8 | — |
| `/.well-known/openid-configuration` | Wo und wie man sich bei dieser Domain anmeldet | OpenID Foundation | 674 | 0,15 % | 0,0–0,8 | — |
| `/openapi.json` | Beschreibung einer Schnittstelle für fremde Programme | OpenAPI Initiative | 650 | 0,15 % | 0,0–0,9 | — |
| `/.well-known/agent-card.json` | Was ein Software-Agent kann und wie man ihn anspricht | A2A Project (Linux Foundation) | 672 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/agent.json` | Fähigkeiten eines Agenten, unter dem alten Dateinamen | A2A Project (Linux Foundation) | 672 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/ai-catalog.json` | Was eine Domain KI-Agenten an Inhalten und Diensten bietet | AI Catalog WG (Linux Foundation), Google, Microsoft | 671 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/ai-plugin.json` | Anleitung, damit ein Chatbot einen Dienst bedienen kann | OpenAI | 656 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/ai.txt` | Dieselben KI-Nutzungsregeln im Sammelordner der Domain | Spawning | 661 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/did.json` | Nachweisbare Identität einer Domain ohne zentrale Stelle | W3C | 672 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/dnt-policy.txt` | Zusage, Besucher nicht über Seiten hinweg zu verfolgen | EFF | 678 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/host-meta` | Verweise auf die weiteren Auskunftsstellen einer Domain | IETF | 670 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/llms.txt` | Inhaltsverzeichnis für Sprachmodelle im Sammelordner | Answer.AI | 658 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/mcp-server` | Wo der Werkzeug-Server einer Domain zu erreichen ist | IETF (individual draft) | 673 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/openapi.json` | Schnittstellen-Beschreibung im Sammelordner der Domain | OpenAPI Initiative | 673 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/openid-federation` | Zu welchem Verbund eine Stelle nachweislich gehört | OpenID Foundation | 677 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/webfinger` | Wer hinter einer Adresse an dieser Domain steckt | IETF | 671 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/x402.json` | Preis und Bezahlweg für maschinelle Abrufe | Coinbase, Cloudflare | 670 | 0,00 % | 0,0–0,6 | — |
| `/ai-plugin.json` | Dieselbe Anleitung für Chatbots, an der Wurzel | OpenAI | 641 | 0,00 % | 0,0–0,6 | — |
| `/swagger.json` | Schnittstellen-Beschreibung unter dem alten Dateinamen | SmartBear (Swagger) | 642 | 0,00 % | 0,0–0,6 | — |

Verbreitung ist der Anteil der Quellen, bei denen wir wirklich nachsehen
durften und die die Route ausgeliefert haben, mit 95-%-Wilson-Intervall.
Quellen, die uns abgewiesen haben (Bot-Wall), den Abruf per robots.txt
untersagen oder nicht erreichbar waren, werden gezählt und gesondert
ausgewiesen — aber eine Nicht-Antwort ist kein „Nein" und steht deshalb
nicht im Nenner.
**`n` ist die Anzahl der Hosts, auf denen diese Route tatsächlich geprobt
wurde — sie unterscheidet sich zwischen den Routen, daher hat jede Zeile
ihren eigenen Nenner und die Zeilen sind nicht direkt miteinander
vergleichbar.**
Noch kein Vorlauf zum Vergleich vorhanden.

<!-- RADAR:END -->
**Was wir abfragen.** Die Tabelle oben ist die vollständige Liste der Routen,
die wir regulär abfragen. Zwei Ergänzungen: Verweisen Dateien Ihrer eigenen
Domain auf eine weitere Datei dort — etwa ein Link in Ihrer `robots.txt` —,
rufen wir diese verwiesene Datei gegebenenfalls einmal ab, höchstens einen
solchen Folge-Abruf je Domain und Lauf, unter denselben `robots.txt`-Regeln.
Und wir fragen je Domain drei DNS-Namenseinträge ab (`_agent`, `_mcp`,
`_index._agents`): reine Namensauflösung, die Ihren Webserver nie berührt.

**Wie eine Route in die Tabelle kommt.** Sie braucht einen benennbaren
Herausgeber oder einen dokumentierten Konsumenten, der sie liest — nicht bloß
ein Format, das irgendwo herumgereicht wird. Der Herausgeber steht in der
Tabelle, damit jede Zeile für sich nachprüfbar ist. Der Zweck sagt, was die
Datei an einem Server tut — er beschreibt sie, er bewertet sie nicht.

## Wie gemessen wird

Die Messung respektiert die `robots.txt`, meldet sich ehrlich mit diesem
Repository als Absender und arbeitet langsam und sparsam. Gemessen werden
ausschließlich öffentliche, für Maschinen bestimmte Konfigurationsdateien —
keine Inhalte.

Die Zahlen oben sind die **August-2026-Basislinie**: ein geschichtetes Panel
von 1.000 Quellen, einmal gemessen. Ab **September 2026** wird das Panel
monatlich gemessen, jede Quelle der größeren Stichprobe einmal pro Quartal.
Mit dem ersten Monatsbericht erscheint zusätzlich ein **14-Monats-Rückblick**
zur Verbreitung von KI-Direktiven (Juni 2025 – Juli 2026), auf Basis von über
**270.000 ausgewerteten robots.txt-Dateien**.

## Wer dahintersteht

Betrieben wird das Radar von **Berger+Team**, einem Freelancer-Kollektiv aus
Südtirol, neben der Arbeit an [btlabs Core](https://btlabs.dev/de). Die Messung
gibt es, weil diese Arbeit Zahlen braucht statt Annahmen: welche Discovery-Wege
tatsächlich genutzt werden und über welche nur geredet wird. Veröffentlicht wird,
was gemessen wurde — auch die Wege, die bei null herauskamen.

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
