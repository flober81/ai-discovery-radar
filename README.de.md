# ai-discovery-radar

[English](README.md) · **Deutsch** · [Italiano](README.it.md)

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22178282.svg)](https://doi.org/10.5281/zenodo.22178282)

**Methode:** Wie diese Zahlen gemessen, klassifiziert und geprüft werden, steht im [Technical Report v1.0](https://doi.org/10.5281/zenodo.22769680) (CC BY 4.0, englisch). Vor dem Zitieren einer Quote lesen.

> **Diese Kennung in Ihren Protokollen gefunden?** Sie können sich mit einer
> einzigen Zeile austragen — siehe [Austragung](#austragung). Kein Konto, kein
> Kontakt, keine Begründung nötig.
>
> <!-- LAST:START -->
> **Wie oft wir vorbeikommen:** rund **16.800 Quellen (Domains) pro Monat**: das Panel von 10.000 Quellen jeden Monat, dazu ein rotierender Block des ~30.000er-Rahmens, jede Block-Quelle höchstens einmal pro Quartal. Einmal im Monat werden 1.000 der Panel-Quellen zusätzlich nach den beobachteten Routen gefragt.
>
> Dazu kommen kleine Entdeckungsläufe auf beliebten Domains außerhalb des Rahmens — höchstens rund 2.000 am Tag — mit den Routen aus den Tabellen unten und der kurzen Liste unter „Nur von den Entdeckungsläufen abgefragt“. Ihre Ergebnisse werden nie veröffentlicht; die Austragung gilt genauso.
> <!-- LAST:END -->

Ein Radar der KI-Discovery-Dateien im öffentlichen Web: welche Routen es gibt
(`robots.txt`, `llms.txt`, `ai-catalog.json`, …), wie weit sie verbreitet sind
und ob sie sich überhaupt abrufen lassen. Jeder Ausschlag ist eine Messung,
keine Meinung.

## Das Radar

<!-- RADAR:START -->
_Lauf **panel-2026-11** · 8603 erreichbare Hosts (8603 registrierbare Domains) · Regelsatz 0.4.0_

| Route | Zweck | Herausgeber | n | Verbreitung | 95 % KI | Trend |
|:--|:--|:--|--:|--:|:--|:-:|
| `/robots.txt` | Welche Bereiche automatische Abrufer betreten dürfen | IETF | 7602 | 84,94 % | 84,1–85,7 | → |
| `/sitemap.xml` | Verzeichnis aller Adressen, die eine Website anbietet | sitemaps.org | 6828 | 54,51 % | 53,3–55,7 | → |
| `/llms.txt` | Inhaltsverzeichnis für Sprachmodelle | Answer.AI | 6567 | 14,76 % | 13,9–15,6 | → |
| `/.well-known/security.txt` | Wohin man eine Sicherheitslücke meldet | IETF | 6805 | 8,38 % | 7,7–9,1 | → |
| `/.well-known/oauth-authorization-server` | Wie die Stelle arbeitet, die Zugangsrechte vergibt | IETF | 6716 | 6,64 % | 6,1–7,3 | → |
| `/.well-known/oauth-protected-resource` | Wo ein Client seine Zugangsberechtigung holt | IETF | 6713 | 6,26 % | 5,7–6,9 | → |
| `/llms-full.txt` | Der gesamte Inhalt einer Website in einer einzigen Datei | Answer.AI | 6556 | 4,51 % | 4,0–5,0 | → |
| `/.well-known/ucp` | Welche Handelsfunktionen ein Händler Agenten anbietet | Universal Commerce Protocol (UCP Tech Council) | 6370 | 3,97 % | 3,5–4,5 | new |
| `/.well-known/gpc.json` | Ob die Seite dem Widerspruch gegen Datenweitergabe folgt | W3C Global Privacy Control | 6742 | 2,85 % | 2,5–3,3 | → |
| `/security.txt` | Wohin man eine Sicherheitslücke meldet, an der Wurzel | IETF | 6981 | 1,25 % | 1,0–1,5 | → |
| `/.well-known/traffic-advice` | Ob ein Zwischenspeicher Seiten vorab laden darf | Google (Private Prefetch Proxy) | 6705 | 1,00 % | 0,8–1,3 | → |
| `/rsl.xml` | Zu welchen Lizenzbedingungen Inhalte genutzt werden dürfen | RSL Collective | 6294 | 0,67 % | 0,5–0,9 | → |
| `/.well-known/tdmrep.json` | Ob Texte und Daten automatisch ausgewertet werden dürfen | W3C TDM Reservation Protocol CG | 6746 | 0,44 % | 0,3–0,6 | → |
| `/.well-known/openid-configuration` | Wo und wie man sich bei dieser Domain anmeldet | OpenID Foundation | 6715 | 0,40 % | 0,3–0,6 | → |
| `/.well-known/api-catalog` | Verzeichnis der Schnittstellen, die eine Domain anbietet | IETF | 6722 | 0,27 % | 0,2–0,4 | → |
| `/ai.txt` | Welche Inhalte für das Training von KI gesperrt sind | Spawning | 6567 | 0,24 % | 0,2–0,4 | → |
| `/.well-known/agent-skills/index.json` | Welche Agent Skills eine Domain anbietet, mit Version und Prüfsumme | Cloudflare (Agent Skills Discovery RFC) | 6364 | 0,19 % | 0,1–0,3 | new |
| `/.well-known/mcp/server-card.json` | Selbstbeschreibung des MCP-Servers einer Site für Clients | no registered publisher — singular variant of MCP SEP-2127, checked by Cloudflare's Agent Readiness Score | 6365 | 0,19 % | 0,1–0,3 | new |
| `/openapi.json` | Beschreibung einer Schnittstelle für fremde Programme | OpenAPI Initiative | 6299 | 0,17 % | 0,1–0,3 | → |
| `/.well-known/ai-catalog.json` | Was eine Domain KI-Agenten an Inhalten und Diensten bietet | AI Catalog WG (Linux Foundation), Google, Microsoft | 6672 | 0,13 % | 0,1–0,3 | → |
| `/.well-known/ai-plugin.json` | Anleitung, damit ein Chatbot einen Dienst bedienen kann | OpenAI | 6506 | 0,09 % | 0,0–0,2 | → |
| `/.well-known/mcp.json` | Welche Werkzeug-Server eine Domain für KI bereitstellt | Model Context Protocol | 6663 | 0,08 % | 0,0–0,2 | → |
| `/.well-known/agent-card.json` | Was ein Software-Agent kann und wie man ihn anspricht | A2A Project (Linux Foundation) | 6673 | 0,06 % | 0,0–0,2 | → |
| `/.well-known/ai.txt` | Dieselben KI-Nutzungsregeln im Sammelordner der Domain | Spawning | 6543 | 0,05 % | 0,0–0,1 | → |
| `/.well-known/host-meta` | Verweise auf die weiteren Auskunftsstellen einer Domain | IETF | 6711 | 0,04 % | 0,0–0,1 | → |
| `/.well-known/did.json` | Nachweisbare Identität einer Domain ohne zentrale Stelle | W3C | 6647 | 0,03 % | 0,0–0,1 | → |
| `/.well-known/dnt-policy.txt` | Zusage, Besucher nicht über Seiten hinweg zu verfolgen | EFF | 6739 | 0,03 % | 0,0–0,1 | → |
| `/swagger.json` | Schnittstellen-Beschreibung unter dem alten Dateinamen | SmartBear (Swagger) | 6226 | 0,03 % | 0,0–0,1 | → |
| `/.well-known/agent.json` | Fähigkeiten eines Agenten, unter dem alten Dateinamen | A2A Project (Linux Foundation) | 6665 | 0,02 % | 0,0–0,1 | → |
| `/.well-known/llms.txt` | Inhaltsverzeichnis für Sprachmodelle im Sammelordner | Answer.AI | 6510 | 0,02 % | 0,0–0,1 | → |
| `/.well-known/webfinger` | Wer hinter einer Adresse an dieser Domain steckt | IETF | 6561 | 0,02 % | 0,0–0,1 | → |
| `/.well-known/mcp-server` | Wo der Werkzeug-Server einer Domain zu erreichen ist | IETF (individual draft) | 6669 | 0,01 % | 0,0–0,1 | → |
| `/.well-known/openapi.json` | Schnittstellen-Beschreibung im Sammelordner der Domain | OpenAPI Initiative | 6625 | 0,00 % | 0,0–0,1 | → |
| `/.well-known/openid-federation` | Zu welchem Verbund eine Stelle nachweislich gehört | OpenID Foundation | 6712 | 0,00 % | 0,0–0,1 | → |
| `/.well-known/x402.json` | Preis und Bezahlweg für maschinelle Abrufe | Coinbase, Cloudflare | 6648 | 0,00 % | 0,0–0,1 | → |
| `/ai-plugin.json` | Dieselbe Anleitung für Chatbots, an der Wurzel | OpenAI | 6255 | 0,00 % | 0,0–0,1 | → |
| `/mcp.json` | Maschinenlesbare Liste der MCP-Endpunkte einer Site, an der Wurzel | Anthropic et al. (MCP) — root-path variant not specified | 6246 | 0,00 % | 0,0–0,1 | → |

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
Ein Pfeil erscheint nur, wenn sich die Intervalle gegenüber **panel-2026-10** nicht überlappen; `→` bedeutet, die Veränderung bleibt innerhalb der Messunsicherheit.
Die Trendpfeile vergleichen das Panel von 10.000 Quellen mit dem Vormonat (dieselbe Liste, derselbe Regelsatz). Der Quartals-Zusammenzug steht als Stand da; sein erster Vergleich ist der Zusammenzug vom Februar 2027.
`new` heißt: die Route wird seit diesem Lauf mitgemessen — es sagt nichts darüber, wann sie im Web zuerst auftrat.
Von den 1623 im ganzen Monatslauf `monat-2026-11-block-c` (Panel und Block) gefundenen `/llms.txt`-Dateien tragen 524 (32,3 %) die Spuren eines Werkzeugs — einen selbstgenannten Erzeuger oder Formulierungen, die sie mit anderen Seiten teilen; die Erzeuger, die sich selbst nennen, sind Erweiterungen für Redaktionssysteme (größte: yoast seo 113, rank math seo 24, all in one seo 17). Die Verbreitungszahl oben zählt Dateien, und das bleibt richtig: eine per Werkzeug ausgerollte Datei ist vorhanden und wird gelesen. Diese Fußnote beantwortet die andere Frage — wie viel an der Zahl Entscheidung ist. Sie ist ein Indiz für diesen Lauf, keine veröffentlichte Quote.
Von den 493 im ganzen Monatslauf `monat-2026-11-block-c` (Panel und Block) gefundenen `/llms-full.txt`-Dateien tragen 351 (71,2 %) die Spuren eines Werkzeugs — einen selbstgenannten Erzeuger oder Formulierungen, die sie mit anderen Seiten teilen. Die Verbreitungszahl oben zählt Dateien, und das bleibt richtig: eine per Werkzeug ausgerollte Datei ist vorhanden und wird gelesen. Diese Fußnote beantwortet die andere Frage — wie viel an der Zahl Entscheidung ist. Sie ist ein Indiz für diesen Lauf, keine veröffentlichte Quote.

### Hinweise zu diesem Lauf

- **Der Cloudflare-Eintrag in der robots.txt ist zurück.** Auf denselben 1.000 Panel-Quellen (robots.txt lesbar) lag der von Cloudflare eingefügte Eintrag bei **7,8 %** im September (55/704, 95-%-KI 6,1–10,0), **2,0 %** im Oktober (14/700, 95-%-KI 1,2–3,3) und **7,2 %** im November (50/695, 95-%-KI 5,5–9,4). Mitte September verschwand die alte Form (Cloudflares Umstellung vom 15. September); eine neue Form („# Training crawlers"), seit Mitte September in einzelnen Dateien zu sehen, breitet sich ab etwa Ende Oktober aus und liegt im November fast wieder auf September-Niveau (41 von 50 in der neuen Form). Oktober → November allein sähe wie ein neuer Höchststand aus; es ist eine Rückkehr.
- Was der neue Eintrag verlangt: im November tragen ihn 439 der 10.000 Panel-Quellen. 420 davon nennen nur KI-Trainings-Crawler (etwa GPTBot, ClaudeBot, CCBot, Google-Extended) und lassen KI-Suche und Abrufe im Auftrag von Nutzern unberührt. 19 bitten zusätzlich KI-Agenten, die für Nutzer abrufen, draußen zu bleiben (ChatGPT-User, Claude-User, Perplexity-User), 6 auch KI-Such-Crawler (OAI-SearchBot, PerplexityBot, Claude-SearchBot). Die robots.txt ist eine Bitte, keine technische Sperre; wir messen nur die robots.txt-Sicht, nicht was eine Firewall tut, und nicht, wer die Einstellung gewählt hat.
- **Voller Rahmen September–November 2026** (alle 30.000 Quellen, jede einmal gemessen; 25.851 erreichbare Organisationen): `/robots.txt` 84,6 % (95-%-KI 84,2–85,1, n 22.968) · `/sitemap.xml` 54,0 % (95-%-KI 53,4–54,7, n 20.515) · `/llms.txt` 14,1 % (95-%-KI 13,6–14,6, n 19.764) · `/.well-known/security.txt` 8,5 % (95-%-KI 8,1–8,9, n 20.503). Das ist ein Stand, kein Trend; sein erster Vergleich ist der Zusammenzug vom Februar 2027.
- Seit Oktober 2026 umfasst das Panel 10.000 Quellen (ein Drittel des Rahmens). Das bisherige Panel von 1.000 Quellen läuft bis Dezember 2026 als Teilmenge darin weiter und wird als eigene Reihe veröffentlicht (`data/panel1000-JJJJ-MM.*`); die beiden Reihen werden nie verkettet.
- Von den 132 Panel-Quellen, die im Oktober den von Cloudflare verwalteten robots.txt-Block trugen, tragen die mit der Marker-Form noch in 20 von 21 lesbaren Dateien einen Block (95,24 %, 95-%-KI 77,3–99,2); die mit der reinen Präambel-Form in 106 von 108 (98,15 %, 95-%-KI 93,5–99,5).
- 1 Datei ließ sich im November nicht lesen (0,77 % der gepaarten Quellen, im ganzen Panel 19,2 %), und 2 Hosts waren nicht erreichbar.
- Eine Gesamtquote geben wir nicht an: Sie würde verdecken, dass sich eine Schreibweise geändert hat, während die Einstellung blieb.
- Content-Signal-Zeilen in der robots.txt: 530 von 6.483 Panel-Hosts (8,18 %, 7,5–8,9); davon 454 in einem vom Anbieter verwalteten Block, 76 (1,17 %, 0,9–1,5) außerhalb.
- Liefert Markdown, wenn Markdown bevorzugt wird: 162 von 6.428 Organisationen (2,52 %, 2,2–2,9).
- Eine Markdown-Fassung vorab anzukündigen ist seltener: `rel="describedby"` 13, `rel="alternate" type="text/markdown"` 3 (eine Untergrenze — zählbar sind nur HTTP-Link-Kopfzeilen).
- Eine einzelne Anfrage kann nicht unterscheiden, ob ein Server aushandelt oder immer Markdown liefert.
- Weil unsere eine Anfrage an die Startseite Markdown bevorzugt, antworteten 162 Startseiten ohne HTML-Kopf; ihre Link-Relationen werden nicht gelesen.
- TDMRep unter Regelsatz 0.4.0: 30 im Panel nach der neuen Regel, 30 nach der alten (siehe Versionshistorie in RULESET.md).
- 2 Organisationen erklären in der robots.txt eine Lizenz (`License:`); 1 davon verweist auf `/rsl.xml`.
- 3 Organisationen kündigen llms.txt in der robots.txt unter einem anderen Pfad als der Wurzel an; die Datei gehört an die Wurzel, deshalb werden sie nicht gezählt.
- DNS: Von 10.000 Panel-Quellen veröffentlichen 0 einen spezifikationskonformen `_agent`-Eintrag; höchstens 1 `_mcp`-Antwort ist weder Wildcard noch SPF.
- `/.well-known/ai-catalog.json`: im festen Panel von 1.000 Quellen 0 von 676 im Oktober und 0 von 675 im November; im Panel von 10.000 Quellen 9 von 6.672 (0,13 %). Lighthouse prüft die Datei seit 2026.
- Dasselbe Panel, im Oktober → im November, nur Hosts, die in beiden Monaten beobachtet wurden (neu / weg von gepaarten Hosts): `/robots.txt` +112 / −42 (n 7.406) · `/sitemap.xml` +54 / −58 (n 6.638) · `/llms.txt` +60 / −20 (n 6.387) · `/.well-known/oauth-protected-resource` +29 / −24 (n 6.549) · `/.well-known/oauth-authorization-server` +26 / −25 (n 6.554) · `/.well-known/security.txt` +18 / −7 (n 6.641).



## Unter Beobachtung (23)

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
- `/agents.md` — Shopify (platform default) and the AGENTS.md convention from code repositories. Wie eine Seite sich gegenüber KI-Agenten beschreibt
- `/.well-known/ard.json` — ARD specification v0.91 (ards-project) — successor path of /.well-known/ai-catalog.json. Inhalte und Dienste einer Domain für KI-Agenten (ARD)

_Beobachtete Routen werden im Monatslauf nicht abgefragt. Unsere Entdeckungsläufe (siehe unten) und eine monatliche Feldprobe auf 1.000 Quellen des Panels fragen sie ab und zählen daraus nichts für diese Seite. Jeder Eintrag trägt im Lab sein Beförderungs-Kriterium._

### Nur von den Entdeckungsläufen abgefragt (27)

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
**Was wir abfragen.** Die Listen oben sind die vollständige Liste der Routen,
die wir abfragen: die gemessenen Routen in jedem Monatslauf; die beobachteten
Routen nur in der monatlichen Feldprobe auf 1.000 Quellen des Panels und in den
Entdeckungsläufen; die Routen unter „Nur von den Entdeckungsläufen abgefragt“
nur dort. Drei Ergänzungen: Ihre Startseite, einmal, um ihre
`<link rel>`-Bekanntgaben zu lesen (die Seite selbst wird verworfen); verweisen
Dateien Ihrer eigenen Domain auf eine weitere Datei dort — etwa ein Link in
Ihrer `robots.txt` —, rufen wir diese verwiesene Datei gegebenenfalls ab,
jede verwiesene Datei höchstens einmal je Lauf, unter denselben
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

Die Zahlen oben stammen aus dem **Panel von 10.000 Quellen**: Seit Oktober 2026 wird ein
geschichtetes Panel von 10.000 Quellen — ein Drittel des Rahmens von 30.000 —
jeden Monat gemessen; das bisherige Panel von 1.000 Quellen läuft darin als
eigene Reihe weiter (siehe Hinweise unter der Tabelle). Die Trendpfeile
vergleichen das Panel mit dem Vormonat; die Regel steht unter der Tabelle. Jede
übrige Quelle des Rahmens wird in jedem Durchgang von drei Monaten einmal gemessen.

**Wofür das Panel steht.** Der Rahmen ist keine Zufallsstichprobe des Webs. Er
besteht aus fünf Schichten: 8.000 Quellen, die in Deutschland, Österreich und der
Schweiz genutzt werden, 3.000 aus Italien, 5.000 aus der weltweiten Spitze,
10.000 aus der weltweiten Breite und 4.000 aus dem Long Tail (wie sie gezogen
werden: [RULESET.md](RULESET.md)). Das Panel übernimmt jede Schicht im selben
Verhältnis, und die Schichten werden nicht gewichtet. Die Zahlen beschreiben
deshalb dieses Panel — nicht „das Web" und nicht „die Top-Sites". Bei einigen
Routen unterscheiden sich die Schichten um das Dreifache und mehr, vor allem weil
sich Plattform-Voreinstellungen im Long Tail häufen.

Der mit dem ersten Monatsbericht angekündigte **14-Monats-Rückblick**
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
sodass jede Block-Quelle einmal pro Quartal an der Reihe ist. Block **c** lief
im November 2026; damit ist der Rahmen zum ersten Mal ganz durchlaufen (September–November 2026). Der Zweck des Block-Laufs ist Abdeckung, nicht Trend.

Alle Reihen liegen in [`data/`](data/): `panel-JJJJ-MM.{json,csv}`,
`panel1000-JJJJ-MM.{json,csv}` und `monat-JJJJ-MM-block-x.{json,csv}`; nach dem letzten Monat jedes Durchlaufs zusätzlich `quartal-JJJJ-qN.{json,csv}`, der volle Rahmen mit jeder Quelle genau einmal (`parts` nennt die drei Läufe, aus denen er besteht). Jede Datei sagt selbst, wann gemessen
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
