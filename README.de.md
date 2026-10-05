# ai-discovery-radar

[English](README.md) · **Deutsch** · [Italiano](README.it.md)

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22178282.svg)](https://doi.org/10.5281/zenodo.22178282)

**Methode:** Wie diese Zahlen gemessen, klassifiziert und geprüft werden, steht im [Technical Report v1.0](https://doi.org/10.5281/zenodo.22769680) (CC BY 4.0, englisch). Vor dem Zitieren einer Quote lesen.

> **Diese Kennung in Ihren Protokollen gefunden?** Sie können sich mit einer
> einzigen Zeile austragen — siehe [Austragung](#austragung). Kein Konto, kein
> Kontakt, keine Begründung nötig.
>
> <!-- LAST:START -->
> **Wie oft wir vorbeikommen:** rund **16.600 Quellen (Domains) pro Monat**: das Panel von 10.000 Quellen jeden Monat, dazu ein rotierender Block des ~30.000er-Rahmens, jede Block-Quelle höchstens einmal pro Quartal. Einmal im Monat werden 1.000 der Panel-Quellen zusätzlich nach den beobachteten Routen gefragt.
>
> Dazu kommen kleine Entdeckungsläufe auf beliebten Domains außerhalb des Rahmens — höchstens rund 2.000 am Tag — mit den Routen aus den Tabellen unten und der kurzen Liste unter „Nur von den Entdeckungsläufen abgefragt“. Ihre Ergebnisse werden nie veröffentlicht; die Austragung gilt genauso.
> <!-- LAST:END -->

Ein Radar der KI-Discovery-Dateien im öffentlichen Web: welche Routen es gibt
(`robots.txt`, `llms.txt`, `ai-catalog.json`, …), wie weit sie verbreitet sind
und ob sie sich überhaupt abrufen lassen. Jeder Ausschlag ist eine Messung,
keine Meinung.

## Das Radar

<!-- RADAR:START -->
_Lauf **panel-2026-10** · 8636 erreichbare Hosts (8636 registrierbare Domains) · Regelsatz 0.4.0_

| Route | Zweck | Herausgeber | n | Verbreitung | 95 % KI | Trend |
|:--|:--|:--|--:|--:|:--|:-:|
| `/robots.txt` | Welche Bereiche automatische Abrufer betreten dürfen | IETF | 7590 | 83,72 % | 82,9–84,5 | — |
| `/sitemap.xml` | Verzeichnis aller Adressen, die eine Website anbietet | sitemaps.org | 6890 | 54,40 % | 53,2–55,6 | — |
| `/llms.txt` | Inhaltsverzeichnis für Sprachmodelle | Answer.AI | 6635 | 14,11 % | 13,3–15,0 | — |
| `/.well-known/security.txt` | Wohin man eine Sicherheitslücke meldet | IETF | 6862 | 8,16 % | 7,5–8,8 | — |
| `/.well-known/oauth-authorization-server` | Wie die Stelle arbeitet, die Zugangsrechte vergibt | IETF | 6782 | 6,56 % | 6,0–7,2 | — |
| `/.well-known/oauth-protected-resource` | Wo ein Client seine Zugangsberechtigung holt | IETF | 6779 | 6,08 % | 5,5–6,7 | — |
| `/llms-full.txt` | Der gesamte Inhalt einer Website in einer einzigen Datei | Answer.AI | 6639 | 4,34 % | 3,9–4,9 | — |
| `/.well-known/gpc.json` | Ob die Seite dem Widerspruch gegen Datenweitergabe folgt | W3C Global Privacy Control | 6800 | 2,84 % | 2,5–3,3 | — |
| `/security.txt` | Wohin man eine Sicherheitslücke meldet, an der Wurzel | IETF | 7050 | 1,21 % | 1,0–1,5 | — |
| `/.well-known/traffic-advice` | Ob ein Zwischenspeicher Seiten vorab laden darf | Google (Private Prefetch Proxy) | 6760 | 0,99 % | 0,8–1,3 | — |
| `/rsl.xml` | Zu welchen Lizenzbedingungen Inhalte genutzt werden dürfen | RSL Collective | 6353 | 0,66 % | 0,5–0,9 | — |
| `/.well-known/openid-configuration` | Wo und wie man sich bei dieser Domain anmeldet | OpenID Foundation | 6771 | 0,37 % | 0,3–0,5 | — |
| `/.well-known/tdmrep.json` | Ob Texte und Daten automatisch ausgewertet werden dürfen | W3C TDM Reservation Protocol CG | 6796 | 0,37 % | 0,2–0,5 | — |
| `/ai.txt` | Welche Inhalte für das Training von KI gesperrt sind | Spawning | 6606 | 0,27 % | 0,2–0,4 | — |
| `/.well-known/api-catalog` | Verzeichnis der Schnittstellen, die eine Domain anbietet | IETF | 6792 | 0,25 % | 0,2–0,4 | — |
| `/openapi.json` | Beschreibung einer Schnittstelle für fremde Programme | OpenAPI Initiative | 6368 | 0,19 % | 0,1–0,3 | — |
| `/.well-known/ai-catalog.json` | Was eine Domain KI-Agenten an Inhalten und Diensten bietet | AI Catalog WG (Linux Foundation), Google, Microsoft | 6733 | 0,09 % | 0,0–0,2 | — |
| `/.well-known/ai-plugin.json` | Anleitung, damit ein Chatbot einen Dienst bedienen kann | OpenAI | 6589 | 0,09 % | 0,0–0,2 | — |
| `/.well-known/mcp.json` | Welche Werkzeug-Server eine Domain für KI bereitstellt | Model Context Protocol | 6726 | 0,07 % | 0,0–0,2 | — |
| `/.well-known/host-meta` | Verweise auf die weiteren Auskunftsstellen einer Domain | IETF | 6783 | 0,06 % | 0,0–0,2 | — |
| `/.well-known/agent-card.json` | Was ein Software-Agent kann und wie man ihn anspricht | A2A Project (Linux Foundation) | 6733 | 0,03 % | 0,0–0,1 | — |
| `/.well-known/ai.txt` | Dieselben KI-Nutzungsregeln im Sammelordner der Domain | Spawning | 6620 | 0,03 % | 0,0–0,1 | — |
| `/.well-known/did.json` | Nachweisbare Identität einer Domain ohne zentrale Stelle | W3C | 6704 | 0,03 % | 0,0–0,1 | — |
| `/swagger.json` | Schnittstellen-Beschreibung unter dem alten Dateinamen | SmartBear (Swagger) | 6302 | 0,03 % | 0,0–0,1 | — |
| `/.well-known/llms.txt` | Inhaltsverzeichnis für Sprachmodelle im Sammelordner | Answer.AI | 6589 | 0,02 % | 0,0–0,1 | — |
| `/.well-known/webfinger` | Wer hinter einer Adresse an dieser Domain steckt | IETF | 6632 | 0,02 % | 0,0–0,1 | — |
| `/mcp.json` | Maschinenlesbare Liste der MCP-Endpunkte einer Site, an der Wurzel | Anthropic et al. (MCP) — root-path variant not specified | 6301 | 0,02 % | 0,0–0,1 | — |
| `/.well-known/agent.json` | Fähigkeiten eines Agenten, unter dem alten Dateinamen | A2A Project (Linux Foundation) | 6729 | 0,01 % | 0,0–0,1 | — |
| `/.well-known/dnt-policy.txt` | Zusage, Besucher nicht über Seiten hinweg zu verfolgen | EFF | 6798 | 0,01 % | 0,0–0,1 | — |
| `/.well-known/mcp-server` | Wo der Werkzeug-Server einer Domain zu erreichen ist | IETF (individual draft) | 6743 | 0,01 % | 0,0–0,1 | — |
| `/.well-known/openapi.json` | Schnittstellen-Beschreibung im Sammelordner der Domain | OpenAPI Initiative | 6709 | 0,00 % | 0,0–0,1 | — |
| `/.well-known/openid-federation` | Zu welchem Verbund eine Stelle nachweislich gehört | OpenID Foundation | 6777 | 0,00 % | 0,0–0,1 | — |
| `/.well-known/x402.json` | Preis und Bezahlweg für maschinelle Abrufe | Coinbase, Cloudflare | 6709 | 0,00 % | 0,0–0,1 | — |
| `/ai-plugin.json` | Dieselbe Anleitung für Chatbots, an der Wurzel | OpenAI | 6305 | 0,00 % | 0,0–0,1 | — |

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
In dieser Ausgabe steht kein Trendpfeil. Die vorangegangenen Läufe decken einen anderen Teil des Rahmens ab; ein Pfeil dazwischen würde zum Teil den Wechsel der Grundgesamtheit messen statt der Veränderung im Web. Ab Dezember vergleicht der Quartals-Zusammenzug Gleiches mit Gleichem — den ganzen Rahmen gegen den ganzen Rahmen —, und dort kommt der Pfeil zurück.
Von den 1535 im ganzen Monatslauf `monat-2026-10-block-b` (Panel und Block) gefundenen `/llms.txt`-Dateien tragen 517 (33,7 %) die Spuren eines Werkzeugs — einen selbstgenannten Erzeuger oder Formulierungen, die sie mit anderen Seiten teilen; die Erzeuger, die sich selbst nennen, sind Erweiterungen für Redaktionssysteme (größte: yoast seo 112, all in one seo 29, rank math seo 19). Die Verbreitungszahl oben zählt Dateien, und das bleibt richtig: eine per Werkzeug ausgerollte Datei ist vorhanden und wird gelesen. Diese Fußnote beantwortet die andere Frage — wie viel an der Zahl Entscheidung ist. Sie ist ein Indiz für diesen Lauf, keine veröffentlichte Quote.
Von den 469 im ganzen Monatslauf `monat-2026-10-block-b` (Panel und Block) gefundenen `/llms-full.txt`-Dateien tragen 343 (73,1 %) die Spuren eines Werkzeugs — einen selbstgenannten Erzeuger oder Formulierungen, die sie mit anderen Seiten teilen. Die Verbreitungszahl oben zählt Dateien, und das bleibt richtig: eine per Werkzeug ausgerollte Datei ist vorhanden und wird gelesen. Diese Fußnote beantwortet die andere Frage — wie viel an der Zahl Entscheidung ist. Sie ist ein Indiz für diesen Lauf, keine veröffentlichte Quote.

### Hinweise zu diesem Lauf

- Seit Oktober 2026 umfasst das Panel 10.000 Quellen (ein Drittel des Rahmens). Das bisherige Panel von 1.000 Quellen läuft bis Dezember 2026 als Teilmenge darin weiter und wird als eigene Reihe veröffentlicht (`data/panel1000-JJJJ-MM.*`); die beiden Reihen werden nie verkettet.
- Von den 238 Panel-Quellen, die im September den von Cloudflare verwalteten robots.txt-Block trugen, tragen die mit der Marker-Form noch in 11 von 149 lesbaren Dateien einen Block (7,38 %, 95-%-KI 4,2–12,7); die mit der reinen Präambel-Form in 38 von 38 (100 %, 95-%-KI 90,8–100,0).
- 47 Dateien ließen sich im Oktober nicht lesen (20,09 % der gepaarten Quellen, im ganzen Panel 20,15 %), und 4 Hosts waren nicht erreichbar.
- Eine Gesamtquote geben wir nicht an: Sie würde verdecken, dass sich eine Schreibweise geändert hat, während die Einstellung blieb.
- Liefert Markdown, wenn Markdown bevorzugt wird: 154 von 6.509 Organisationen (2,37 %, 2,0–2,8).
- Eine Markdown-Fassung vorab anzukündigen ist seltener: `rel="describedby"` 9, `rel="alternate" type="text/markdown"` 2 (eine Untergrenze — zählbar sind nur HTTP-Link-Kopfzeilen).
- Eine einzelne Anfrage kann nicht unterscheiden, ob ein Server aushandelt oder immer Markdown liefert.
- Weil unsere eine Anfrage an die Startseite Markdown bevorzugt, antworteten 154 Startseiten ohne HTML-Kopf; ihre Link-Relationen werden nicht gelesen.
- TDMRep unter Regelsatz 0.4.0: 25 im Panel nach der neuen Regel, 25 nach der alten (siehe Versionshistorie in RULESET.md).
- 2 Organisationen erklären in der robots.txt eine Lizenz (`License:`); 1 davon verweist auf `/rsl.xml`.
- 3 Organisationen kündigen llms.txt in der robots.txt unter einem anderen Pfad als der Wurzel an; die Datei gehört an die Wurzel, deshalb werden sie nicht gezählt.
- DNS: Von 10.000 Panel-Quellen veröffentlichen 0 einen spezifikationskonformen `_agent`-Eintrag und 0 einen `_mcp`-Eintrag, der sich von Wildcard- oder Verifikationsantworten unterscheiden lässt.
- `/.well-known/ai-catalog.json`: im festen Panel von 1.000 Quellen 0 von 675 im September und 0 von 676 im Oktober; im Panel von 10.000 Quellen 6 von 6.733 (0,09 %). Lighthouse prüft die Datei seit 2026.



## Unter Beobachtung (24)

**Bestätigt** — registriert (IANA) oder RFC, im Feld noch kaum zu sehen:

- `/.well-known/nostr.json` — Nostr Developer Community (NIP-05). Nachweis, dass ein öffentlicher Schlüssel zu einem Namen dieser Domain gehört
- `/.well-known/vacation-rental.json` — Vacation Rental Protocol (single registrant). Entdeckungsdokument für kryptographisch signierte Buchungsangebote
- `/.well-known/xregistry` — xRegistry Authors (CNCF Sandbox). Einstiegspunkt eines erweiterbaren Registrys für Schemata und Events
- `/.well-known/host-meta.json` — IETF. JSON-Zwilling der host-meta-Verweise
- `/.well-known/open-resource-discovery` — SAP SE (Open Resource Discovery). Ein Einstiegspunkt, der die Schnittstellen und Ereignisse eines Systems zur Entdeckung auflistet

**Im Entstehen** — Feldsignale oder Entwürfe, noch ohne Registrierung:

- `/.well-known/atproto-did` — AT Protocol (Bluesky). Löst ein Domain-Handle auf eine dezentrale Identität auf
- `/server-card.json` — no nameable publisher (circulating agent spec). Vorgeschlagene Selbstbeschreibungs-Karte für Agenten-Server
- `/product.xml` — no publisher — emerging commerce convention. Produktlisten, die Shops für maschinelle Leser verlinken
- `Signposting (Link header: describedby/cite-as/linkset)` — FAIR Signposting Profile (scholarly repository community). Maschinenlesbare Verweise wissenschaftlicher Seiten auf ihre Metadaten und Volltexte
- `/.well-known/jwt-vc-issuer` — IETF (OAuth WG, draft stage). Wo ein Prüfer die Schlüssel eines Ausstellers verifizierbarer Nachweise findet
- `/.well-known/ai` — IETF draft (AI Discovery Endpoint). Vorgeschlagene maschinenlesbare Fähigkeits-Beschreibung für KI-Agenten
- `_agent (DNS TXT record, no HTTP route)` — IETF draft (Agent Identity and Discovery, AID). DNS-Eintrag, der Agenten-Identitäts-Entdeckung vorschlägt
- `Content-Usage (robots.txt directive + HTTP header, no path)` — IETF AIPREF WG (draft-ietf-aipref-attach, WG-adopted, Standards Track). Direktive, die sagt, was KI mit den Inhalten tun darf
- `Schemamap (robots.txt directive; target URL free, conventionally /schema.txt)` — SCHEMA.TXT (specification on GitHub). Direktive, die Maschinen auf die Schema-Karte einer Site verweist
- `/.well-known/did-configuration.json` — Decentralized Identity Foundation (DIF). Nachweis, der eine Domain mit dezentralen Identitäten verknüpft
- `_apertoid (DNS TXT record, no HTTP route)` — ApertoID (single vendor). DNS-Eintrag eines entstehenden Offene-Identität-Vorschlags
- `_x402 (DNS-TXT) + /.well-known/x402` — Individual draft (W. Hawkins) for the Coinbase/Cloudflare x402. DNS- und Web-Entdeckung von x402-Zahlungs-Endpunkten
- `_agents / AIDISCA+AIINDEX (new DNS RR types)` — Verisign (individual draft). Vorgeschlagene DNS-Eintragstypen für Agenten-Entdeckung
- `Link rel=client-ranges (HTTP Link header)` — Individual draft (Google/Ericsson authors). Kopfzeile, die Clients auf deklarierte IP-Bereiche verweist
- `Agentmap (robots.txt directive; target URL free)` — AI Catalog Working Group (Linux Foundation) — Agentic Resource Discovery spec. Eine robots.txt-Zeile, die Maschinen zum KI-Ressourcenkatalog einer Site fuehrt
- `Archive-Embargo / Embargo-Allow (robots.txt directives, no path)` — Individual draft (M. Nottingham, M. Thomson — HTTP WG environment). robots.txt-Zeilen, die steuern, ab wann archivierte Kopien einer Site veroeffentlicht werden duerfen
- `/agents.md` — Shopify (Plattform-Vorgabe) sowie die AGENTS.md-Konvention aus Code-Ablagen. Wie eine Seite sich gegenüber KI-Agenten beschreibt
- `/.well-known/ucp` — Universal Commerce Protocol (UCP Tech Council). Welche Handelsfunktionen ein Händler Agenten anbietet
- `/.well-known/agent-skills/index.json` — Cloudflare (Agent Skills Discovery RFC, Status Draft). Welche Agent Skills eine Domain anbietet, mit Version und Prüfsumme

_Beobachtete Routen werden im Monatslauf nicht abgefragt. Unsere Entdeckungsläufe (siehe unten) und eine monatliche Feldprobe auf 1.000 Quellen des Panels fragen sie ab und zählen daraus nichts für diese Seite. Jeder Eintrag trägt im Lab sein Beförderungs-Kriterium._

### Nur von den Entdeckungsläufen abgefragt (20)

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
**Was wir abfragen.** Die Listen oben sind die vollständige Liste der Routen,
die wir abfragen: die gemessenen Routen in jedem Monatslauf; die beobachteten
Routen nur in der monatlichen Feldprobe auf 1.000 Quellen des Panels und in den
Entdeckungsläufen; die Routen unter „Nur von den Entdeckungsläufen abgefragt“
nur dort. Drei Ergänzungen: Ihre Startseite, einmal, um ihre
`<link rel>`-Bekanntgaben zu lesen (die Seite selbst wird verworfen); verweisen
Dateien Ihrer eigenen Domain auf eine weitere Datei dort — etwa ein Link in
Ihrer `robots.txt` —, rufen wir diese verwiesene Datei gegebenenfalls einmal ab,
höchstens einen solchen Folge-Abruf je Domain und Lauf, unter denselben
`robots.txt`-Regeln; und je Domain drei DNS-Namenseinträge (`_agent`, `_mcp`,
`_index._agents`): reine Namensauflösung, die Ihren Webserver nie berührt.
Nichts davon wird als Inhalt veröffentlicht — nur Anzahlen und Anteile je
Route, und aus Feldprobe und Entdeckungsläufen gar nichts.

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

Die Zahlen oben sind das **Oktober-2026-Panel**: Seit Oktober 2026 wird ein
geschichtetes Panel von 10.000 Quellen — ein Drittel des Rahmens von 30.000 —
jeden Monat gemessen; das bisherige Panel von 1.000 Quellen läuft darin als
eigene Reihe weiter (siehe Hinweise unter der Tabelle). Diese Ausgabe zeigt
keinen Trendpfeil; warum, steht unter der Tabelle. Jede übrige Quelle des
Rahmens wird einmal pro Quartal gemessen. Der mit dem ersten Monatsbericht angekündigte **14-Monats-Rückblick**
zur Verbreitung von KI-Direktiven liegt vor:
[REVIEW-2025-2026.md](REVIEW-2025-2026.md) — acht Common-Crawl-Stände, Juni 2025
bis Juli 2026: Antwort-Kopfzeilen von **3,6 Millionen Seiten** (2,7 Millionen
Organisationen), dazu ein separater Scan von über **270.000 robots.txt-Dateien**.

## Datendateien pro Monat

Die Tabelle oben ist das **Panel**: 10.000 feste Quellen (ein Drittel des
Rahmens), jeden Monat gemessen. Veränderung zeigt nur Panel gegen Panel, und
nur innerhalb einer Reihe: Bis Dezember 2026 erscheint das bisherige Panel von
1.000 Quellen daneben als eigene Reihe — die einzige, die bis August 2026
zurückreicht —, und die beiden Reihen werden nie verkettet. Jeden Monat wird im
selben Lauf außerdem ein **Block** der größeren Stichprobe von 30.000 gemessen —
sie ist in drei Blöcke (a, b, c) geteilt, die durch das Quartal rotieren,
sodass jede Block-Quelle einmal pro Quartal an der Reihe ist. Block **b** lief
im Oktober 2026. Der Zweck des Block-Laufs ist Abdeckung, nicht Trend.

Alle Reihen liegen in [`data/`](data/): `panel-JJJJ-MM.{json,csv}`,
`panel1000-JJJJ-MM.{json,csv}` und `monat-JJJJ-MM-block-x.{json,csv}`. Jede Datei sagt selbst, wann gemessen
wurde und ob sie vollständig ist (`measurement_window.status`); wie die
Stichprobe geteilt wird, steht in [RULESET.md](RULESET.md).

## Wer dahintersteht

Betrieben wird das Radar von **Berger+Team**, einem Freelancer-Kollektiv aus
Südtirol, neben der Arbeit an [btlabs Core](https://btlabs.dev/de). Die Messung
gibt es, weil diese Arbeit Zahlen braucht statt Annahmen: welche Discovery-Wege
tatsächlich genutzt werden und über welche nur geredet wird. Veröffentlicht wird,
was gemessen wurde — auch die Wege, die bei null herauskamen.

## Austragung

Keine Rückfragen, keine Begründung nötig. Ein Weg genügt:

1. E-Mail an **florian@berger.team** mit der Domain — dafür brauchen Sie
   kein GitHub-Konto, **oder**
2. ein Issue in diesem Repository mit der Domain, **oder**
3. eine `Disallow`-Regel für unsere Kennung `ai-discovery-radar` in Ihrer `robots.txt` — das wirkt
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
