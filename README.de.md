# ai-discovery-radar

[English](README.md) · **Deutsch** · [Italiano](README.it.md)

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22178282.svg)](https://doi.org/10.5281/zenodo.22178282)

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
_Lauf **panel-2026-09** · 853 erreichbare Hosts (853 registrierbare Domains) · Regelsatz 0.3.2_

| Route | Zweck | Herausgeber | n | Verbreitung | 95 % KI | Trend |
|:--|:--|:--|--:|--:|:--|:-:|
| `/robots.txt` | Welche Bereiche automatische Abrufer betreten dürfen | IETF | 761 | 86,20 % | 83,6–88,5 | → |
| `/sitemap.xml` | Verzeichnis aller Adressen, die eine Website anbietet | sitemaps.org | 686 | 55,39 % | 51,7–59,1 | → |
| `/llms.txt` | Inhaltsverzeichnis für Sprachmodelle | Answer.AI | 669 | 13,45 % | 11,1–16,2 | → |
| `/.well-known/security.txt` | Wohin man eine Sicherheitslücke meldet | IETF | 684 | 7,02 % | 5,3–9,2 | → |
| `/.well-known/oauth-authorization-server` | Wie die Stelle arbeitet, die Zugangsrechte vergibt | IETF | 678 | 5,16 % | 3,7–7,1 | → |
| `/.well-known/oauth-protected-resource` | Wo ein Client seine Zugangsberechtigung holt | IETF | 678 | 4,87 % | 3,5–6,8 | → |
| `/llms-full.txt` | Der gesamte Inhalt einer Website in einer einzigen Datei | Answer.AI | 666 | 4,80 % | 3,4–6,7 | → |
| `/.well-known/gpc.json` | Ob die Seite dem Widerspruch gegen Datenweitergabe folgt | W3C Global Privacy Control | 682 | 2,79 % | 1,8–4,3 | → |
| `/.well-known/traffic-advice` | Ob ein Zwischenspeicher Seiten vorab laden darf | Google (Private Prefetch Proxy) | 673 | 1,34 % | 0,7–2,5 | → |
| `/security.txt` | Wohin man eine Sicherheitslücke meldet, an der Wurzel | IETF | 698 | 1,15 % | 0,6–2,2 | → |
| `/rsl.xml` | Zu welchen Lizenzbedingungen Inhalte genutzt werden dürfen | RSL Collective | 641 | 0,78 % | 0,3–1,8 | → |
| `/ai.txt` | Welche Inhalte für das Training von KI gesperrt sind | Spawning | 668 | 0,45 % | 0,2–1,3 | → |
| `/openapi.json` | Beschreibung einer Schnittstelle für fremde Programme | OpenAPI Initiative | 651 | 0,31 % | 0,1–1,1 | → |
| `/.well-known/openid-configuration` | Wo und wie man sich bei dieser Domain anmeldet | OpenID Foundation | 678 | 0,29 % | 0,1–1,1 | → |
| `/.well-known/tdmrep.json` | Ob Texte und Daten automatisch ausgewertet werden dürfen | W3C TDM Reservation Protocol CG | 685 | 0,29 % | 0,1–1,1 | → |
| `/.well-known/agent.json` | Fähigkeiten eines Agenten, unter dem alten Dateinamen | A2A Project (Linux Foundation) | 676 | 0,15 % | 0,0–0,8 | → |
| `/.well-known/api-catalog` | Verzeichnis der Schnittstellen, die eine Domain anbietet | IETF | 676 | 0,15 % | 0,0–0,8 | → |
| `/.well-known/mcp.json` | Welche Werkzeug-Server eine Domain für KI bereitstellt | Model Context Protocol | 676 | 0,15 % | 0,0–0,8 | → |
| `/.well-known/agent-card.json` | Was ein Software-Agent kann und wie man ihn anspricht | A2A Project (Linux Foundation) | 675 | 0,00 % | 0,0–0,6 | → |
| `/.well-known/ai-catalog.json` | Was eine Domain KI-Agenten an Inhalten und Diensten bietet | AI Catalog WG (Linux Foundation), Google, Microsoft | 675 | 0,00 % | 0,0–0,6 | → |
| `/.well-known/ai-plugin.json` | Anleitung, damit ein Chatbot einen Dienst bedienen kann | OpenAI | 661 | 0,00 % | 0,0–0,6 | → |
| `/.well-known/ai.txt` | Dieselben KI-Nutzungsregeln im Sammelordner der Domain | Spawning | 664 | 0,00 % | 0,0–0,6 | → |
| `/.well-known/did.json` | Nachweisbare Identität einer Domain ohne zentrale Stelle | W3C | 674 | 0,00 % | 0,0–0,6 | → |
| `/.well-known/dnt-policy.txt` | Zusage, Besucher nicht über Seiten hinweg zu verfolgen | EFF | 681 | 0,00 % | 0,0–0,6 | → |
| `/.well-known/host-meta` | Verweise auf die weiteren Auskunftsstellen einer Domain | IETF | 675 | 0,00 % | 0,0–0,6 | → |
| `/.well-known/llms.txt` | Inhaltsverzeichnis für Sprachmodelle im Sammelordner | Answer.AI | 663 | 0,00 % | 0,0–0,6 | → |
| `/.well-known/mcp-server` | Wo der Werkzeug-Server einer Domain zu erreichen ist | IETF (individual draft) | 675 | 0,00 % | 0,0–0,6 | → |
| `/.well-known/openapi.json` | Schnittstellen-Beschreibung im Sammelordner der Domain | OpenAPI Initiative | 676 | 0,00 % | 0,0–0,6 | → |
| `/.well-known/openid-federation` | Zu welchem Verbund eine Stelle nachweislich gehört | OpenID Foundation | 678 | 0,00 % | 0,0–0,6 | → |
| `/.well-known/webfinger` | Wer hinter einer Adresse an dieser Domain steckt | IETF | 674 | 0,00 % | 0,0–0,6 | → |
| `/.well-known/x402.json` | Preis und Bezahlweg für maschinelle Abrufe | Coinbase, Cloudflare | 675 | 0,00 % | 0,0–0,6 | → |
| `/ai-plugin.json` | Dieselbe Anleitung für Chatbots, an der Wurzel | OpenAI | 643 | 0,00 % | 0,0–0,6 | → |
| `/mcp.json` | Maschinenlesbare Liste der MCP-Endpunkte einer Site, an der Wurzel | Anthropic et al. (MCP) — root-path variant not specified | 642 | 0,00 % | 0,0–0,6 | new |
| `/swagger.json` | Schnittstellen-Beschreibung unter dem alten Dateinamen | SmartBear (Swagger) | 643 | 0,00 % | 0,0–0,6 | → |

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
Ein Pfeil erscheint nur, wenn sich die Intervalle gegenüber **panel-2026-08** nicht überlappen; `→` bedeutet, die Veränderung bleibt innerhalb der Messunsicherheit.
Der Vorlauf wurde unter Regelsatz 0.3.1 gerechnet, dieser Lauf unter 0.3.2 — was sich geändert hat, steht in RULESET.md; der erste reguläre Monatsvergleich ist der nächste Lauf.
`new` heißt: die Route wird seit diesem Lauf mitgemessen — es sagt nichts darüber, wann sie im Web zuerst auftrat.



## Unter Beobachtung (21)

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

_Beobachtet heißt beobachtet — nichts davon wird oben gemessen oder gezählt. Jeder Eintrag trägt im Lab sein Beförderungs-Kriterium._
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

Die Zahlen oben sind das **September-2026-Panel**: Dasselbe geschichtete Panel
von 1.000 Quellen wird jeden Monat gemessen; die Spalte **Trend** vergleicht
jede Route mit dem Vormonat (August 2026 war die erste Messung dieses Panels,
gerechnet unter einem früheren Regelsatz — siehe Hinweis unter der Tabelle).
Jede Quelle der größeren Stichprobe von 30.000 wird einmal pro Quartal
gemessen. Der mit dem ersten Monatsbericht angekündigte **14-Monats-Rückblick**
zur Verbreitung von KI-Direktiven liegt vor:
[REVIEW-2025-2026.md](REVIEW-2025-2026.md) — acht Common-Crawl-Stände, Juni 2025
bis Juli 2026: Antwort-Kopfzeilen von **3,6 Millionen Seiten** (2,7 Millionen
Organisationen), dazu ein separater Scan von über **270.000 robots.txt-Dateien**.

## Zwei Datendateien pro Monat

Die Tabelle oben ist das **Panel**: 1.000 feste Quellen, jeden Monat gemessen,
die einzige Reihe, in der ein Pfeil eine Veränderung bedeutet. Daneben wird
jeden Monat ein **Block** der größeren Stichprobe von 30.000 gemessen — sie ist
in drei Blöcke (a, b, c) geteilt, die durch das Quartal rotieren, sodass jede
Domain einmal pro Quartal an der Reihe ist. Block **a** lief im September 2026.
Ein Block-Lauf umfasst rund zehnmal so viele Hosts wie das Panel; seine
Intervalle sind entsprechend eng, sein Zweck ist Abdeckung, nicht Trend.

Beide Läufe liegen in [`data/`](data/): `panel-JJJJ-MM.{json,csv}` und
`monat-JJJJ-MM-block-x.{json,csv}`. Jede Datei sagt selbst, wann gemessen
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
