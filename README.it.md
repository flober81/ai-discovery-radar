# ai-discovery-radar

[English](README.md) · [Deutsch](README.de.md) · **Italiano**

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22178282.svg)](https://doi.org/10.5281/zenodo.22178282)

**Metodo:** come questi numeri vengono misurati, classificati e verificati è documentato nel [Technical Report v1.0](https://doi.org/10.5281/zenodo.22769680) (CC BY 4.0, in inglese). Da leggere prima di citare una quota.

> **Trovato questo identificativo nei log del vostro server?** Potete escludervi
> con una sola riga — vedi [Come escludersi](#come-escludersi). Nessun account,
> nessun contatto, nessuna motivazione richiesta.
>
> <!-- LAST:START -->
> **Quanto spesso passiamo:** circa **16.600 fonti (domini) al mese**: il panel di 10.000 fonti ogni mese, più un blocco a rotazione del quadro di ~30.000 fonti, ogni fonte di blocco al massimo una volta a trimestre. Una volta al mese, a 1.000 fonti del panel vengono richieste anche le route sotto osservazione.
>
> In più, piccole rilevazioni esplorative visitano domini popolari al di fuori del quadro — al massimo circa 2.000 al giorno — con le route delle tabelle qui sotto più il breve elenco «Richieste solo dalle rilevazioni esplorative». I loro risultati non vengono mai pubblicati; vale la stessa esclusione.
> <!-- LAST:END -->

Un radar dei file di AI discovery sul web pubblico: quali route esistono
(`robots.txt`, `llms.txt`, `ai-catalog.json`, …), quanto sono diffuse e se sono
davvero scaricabili. Ogni segnale è una misurazione, non un'opinione.

## Il radar

<!-- RADAR:START -->
_Misurazione **panel-2026-10** · 8636 host raggiungibili (8636 domini registrabili) · regole 0.4.0_

| Route | Scopo | Editore | n | Diffusione | IC 95 % | Tendenza |
|:--|:--|:--|--:|--:|:--|:-:|
| `/robots.txt` | Quali aree di un sito i crawler possono visitare | IETF | 7590 | 83,72 % | 82,9–84,5 | — |
| `/sitemap.xml` | L'elenco di tutti gli indirizzi che un sito offre | sitemaps.org | 6890 | 54,40 % | 53,2–55,6 | — |
| `/llms.txt` | Un indice dei contenuti per i modelli linguistici | Answer.AI | 6635 | 14,11 % | 13,3–15,0 | — |
| `/.well-known/security.txt` | Dove segnalare una vulnerabilità di sicurezza | IETF | 6862 | 8,16 % | 7,5–8,8 | — |
| `/.well-known/oauth-authorization-server` | Come funziona il servizio che concede l'accesso | IETF | 6782 | 6,56 % | 6,0–7,2 | — |
| `/.well-known/oauth-protected-resource` | Dove un client ottiene l'autorizzazione all'accesso | IETF | 6779 | 6,08 % | 5,5–6,7 | — |
| `/llms-full.txt` | L'intero contenuto di un sito in un unico file | Answer.AI | 6639 | 4,34 % | 3,9–4,9 | — |
| `/.well-known/gpc.json` | Se il sito rispetta l'opt-out sulla condivisione dei dati | W3C Global Privacy Control | 6800 | 2,84 % | 2,5–3,3 | — |
| `/security.txt` | Dove segnalare una vulnerabilità, alla radice del sito | IETF | 7050 | 1,21 % | 1,0–1,5 | — |
| `/.well-known/traffic-advice` | Se un proxy di cache può precaricare le pagine | Google (Private Prefetch Proxy) | 6760 | 0,99 % | 0,8–1,3 | — |
| `/rsl.xml` | A quali condizioni di licenza si possono usare i contenuti | RSL Collective | 6353 | 0,66 % | 0,5–0,9 | — |
| `/.well-known/openid-configuration` | Dove e come si accede a questo dominio | OpenID Foundation | 6771 | 0,37 % | 0,3–0,5 | — |
| `/.well-known/tdmrep.json` | Se testi e dati possono essere estratti automaticamente | W3C TDM Reservation Protocol CG | 6796 | 0,37 % | 0,2–0,5 | — |
| `/ai.txt` | Quali contenuti sono esclusi dall'addestramento di AI | Spawning | 6606 | 0,27 % | 0,2–0,4 | — |
| `/.well-known/api-catalog` | L'elenco delle interfacce offerte da un dominio | IETF | 6792 | 0,25 % | 0,2–0,4 | — |
| `/openapi.json` | La descrizione di un'interfaccia per altri programmi | OpenAPI Initiative | 6368 | 0,19 % | 0,1–0,3 | — |
| `/.well-known/ai-catalog.json` | Quali contenuti e servizi un dominio offre agli agenti AI | AI Catalog WG (Linux Foundation), Google, Microsoft | 6733 | 0,09 % | 0,0–0,2 | — |
| `/.well-known/ai-plugin.json` | Istruzioni perché un chatbot possa usare un servizio | OpenAI | 6589 | 0,09 % | 0,0–0,2 | — |
| `/.well-known/mcp.json` | Quali tool server un dominio mette a disposizione per AI | Model Context Protocol | 6726 | 0,07 % | 0,0–0,2 | — |
| `/.well-known/host-meta` | I rimandi agli altri punti informativi di un dominio | IETF | 6783 | 0,06 % | 0,0–0,2 | — |
| `/.well-known/agent-card.json` | Cosa sa fare un agente software e come interpellarlo | A2A Project (Linux Foundation) | 6733 | 0,03 % | 0,0–0,1 | — |
| `/.well-known/ai.txt` | Le stesse regole d'uso per AI nella cartella well-known | Spawning | 6620 | 0,03 % | 0,0–0,1 | — |
| `/.well-known/did.json` | L'identità verificabile di un dominio senza enti centrali | W3C | 6704 | 0,03 % | 0,0–0,1 | — |
| `/swagger.json` | La descrizione dell'interfaccia col vecchio nome di file | SmartBear (Swagger) | 6302 | 0,03 % | 0,0–0,1 | — |
| `/.well-known/llms.txt` | Un indice per i modelli linguistici, in well-known | Answer.AI | 6589 | 0,02 % | 0,0–0,1 | — |
| `/.well-known/webfinger` | Chi sta dietro un indirizzo di questo dominio | IETF | 6632 | 0,02 % | 0,0–0,1 | — |
| `/mcp.json` | L'elenco leggibile dalle macchine degli endpoint MCP, alla radice | Anthropic et al. (MCP) — root-path variant not specified | 6301 | 0,02 % | 0,0–0,1 | — |
| `/.well-known/agent.json` | Le capacità di un agente, col vecchio nome di file | A2A Project (Linux Foundation) | 6729 | 0,01 % | 0,0–0,1 | — |
| `/.well-known/dnt-policy.txt` | La promessa di non tracciare i visitatori tra i siti | EFF | 6798 | 0,01 % | 0,0–0,1 | — |
| `/.well-known/mcp-server` | Dove raggiungere il tool server di un dominio | IETF (individual draft) | 6743 | 0,01 % | 0,0–0,1 | — |
| `/.well-known/openapi.json` | La descrizione dell'interfaccia nella cartella well-known | OpenAPI Initiative | 6709 | 0,00 % | 0,0–0,1 | — |
| `/.well-known/openid-federation` | A quale federazione appartiene un soggetto, con prova | OpenID Foundation | 6777 | 0,00 % | 0,0–0,1 | — |
| `/.well-known/x402.json` | Prezzo e modo di pagamento per le richieste automatiche | Coinbase, Cloudflare | 6709 | 0,00 % | 0,0–0,1 | — |
| `/ai-plugin.json` | Le stesse istruzioni per chatbot, alla radice del sito | OpenAI | 6305 | 0,00 % | 0,0–0,1 | — |

La diffusione è la quota delle fonti che abbiamo potuto davvero consultare
e che hanno restituito la route, con intervallo di Wilson al 95 %. Le fonti
che ci hanno respinto (bot wall), che vietano il prelievo via robots.txt o
che non erano raggiungibili vengono contate e riportate a parte — ma una
non-risposta non è un «no», quindi non entra nel denominatore.
**`n` è il numero di host su cui la route è stata effettivamente testata.
Cambia da una route all'altra, quindi ogni riga ha il proprio denominatore
e le righe non sono direttamente confrontabili tra loro.**
In questa edizione non compare la freccia di tendenza. Le misurazioni precedenti coprono una parte diversa del campione, quindi una freccia tra di esse misurerebbe in parte il cambio di popolazione anziché il cambiamento sul web. Da dicembre il consolidamento trimestrale confronta ciò che è confrontabile — l'intero campione contro l'intero campione — e lì la freccia torna.
Dei 1535 file `/llms.txt` trovati nell'intera misurazione mensile `monat-2026-10-block-b` (panel e blocco), 517 (33,7 %) portano i segni di uno strumento: un generatore che si dichiara o formulazioni condivise con altri siti; i generatori che si dichiarano sono estensioni per sistemi di gestione dei contenuti (i maggiori: yoast seo 112, all in one seo 29, rank math seo 19). Il dato di diffusione qui sopra conta i file, e resta corretto così: un file distribuito da uno strumento esiste e viene letto. Questa nota risponde all'altra domanda — quanta parte del numero è una decisione. È un indizio per questa misurazione, non un tasso pubblicato.
Dei 469 file `/llms-full.txt` trovati nell'intera misurazione mensile `monat-2026-10-block-b` (panel e blocco), 343 (73,1 %) portano i segni di uno strumento: un generatore che si dichiara o formulazioni condivise con altri siti. Il dato di diffusione qui sopra conta i file, e resta corretto così: un file distribuito da uno strumento esiste e viene letto. Questa nota risponde all'altra domanda — quanta parte del numero è una decisione. È un indizio per questa misurazione, non un tasso pubblicato.

### Note su questa rilevazione

- Da ottobre 2026 il panel comprende 10.000 fonti (un terzo del quadro). Il panel precedente di 1.000 fonti prosegue al suo interno come sottoinsieme fino a dicembre 2026 ed è pubblicato come serie a sé (`data/panel1000-AAAA-MM.*`); le due serie non vengono mai concatenate.
- Delle 238 fonti del panel che a settembre riportavano il blocco robots.txt gestito da Cloudflare, quelle con la forma a marcatori riportano ancora un blocco in 11 file leggibili su 149 (7,38 %, IC 95 % 4,2–12,7); quelle con la sola forma a preambolo in 38 su 38 (100 %, IC 95 % 90,8–100,0).
- 47 file non erano leggibili a ottobre (20,09 % delle fonti appaiate, contro 20,15 % nell'intero panel) e 4 host non erano raggiungibili.
- Non indichiamo un tasso complessivo: nasconderebbe che è cambiata una notazione mentre l'impostazione è rimasta.
- Restituisce Markdown quando si preferisce Markdown: 154 organizzazioni su 6.509 (2,37 %, 2,0–2,8).
- Annunciare in anticipo una versione Markdown è più raro: `rel="describedby"` 9, `rel="alternate" type="text/markdown"` 2 (un limite inferiore — sono conteggiabili solo le intestazioni HTTP Link).
- Una singola richiesta non può distinguere se un server negozia o restituisce sempre Markdown.
- Poiché la nostra unica richiesta alla home page preferisce Markdown, 154 home page hanno risposto senza intestazione HTML; le loro relazioni di link non vengono lette.
- TDMRep con le regole 0.4.0: 25 nel panel secondo la nuova regola, 25 secondo la precedente (vedi la cronologia delle versioni in RULESET.md).
- 2 organizzazioni dichiarano una licenza nel robots.txt (`License:`); 1 di esse rimanda a `/rsl.xml`.
- 3 organizzazioni annunciano llms.txt nel robots.txt con un percorso diverso dalla radice; il file va nella radice, quindi non vengono conteggiate.
- DNS: su 10.000 fonti del panel, 0 pubblicano un record `_agent` conforme alla specifica e 0 un record `_mcp` distinguibile da risposte wildcard o di verifica.
- `/.well-known/ai-catalog.json`: nel panel fisso di 1.000 fonti 0 su 675 a settembre e 0 su 676 a ottobre; nel panel di 10.000 fonti 6 su 6.733 (0,09 %). Lighthouse controlla il file dal 2026.



## Sotto osservazione (24)

**Confermate** — registrate (IANA) o RFC, quasi assenti sul campo:

- `/.well-known/nostr.json` — Nostr Developer Community (NIP-05). Prova che una chiave pubblica appartiene a un nome di questo dominio
- `/.well-known/vacation-rental.json` — Vacation Rental Protocol (single registrant). Documento di scoperta per offerte di soggiorno firmate crittograficamente
- `/.well-known/xregistry` — xRegistry Authors (CNCF Sandbox). Punto d'ingresso di un registro estensibile per schemi ed eventi
- `/.well-known/host-meta.json` — IETF. Il gemello JSON dei rimandi host-meta
- `/.well-known/open-resource-discovery` — SAP SE (Open Resource Discovery). Un punto d'ingresso che elenca le interfacce e gli eventi che un sistema espone per la scoperta

**In formazione** — segnali dal campo o bozze, senza registrazione:

- `/.well-known/atproto-did` — AT Protocol (Bluesky). Risolve un handle di dominio in un'identità decentralizzata
- `/server-card.json` — no nameable publisher (circulating agent spec). Una proposta di scheda descrittiva per server rivolti agli agenti
- `/product.xml` — no publisher — emerging commerce convention. Elenchi di prodotti che i negozi collegano per i lettori automatici
- `Signposting (Link header: describedby/cite-as/linkset)` — FAIR Signposting Profile (scholarly repository community). Rimandi leggibili dalle macchine dalle pagine scientifiche ai loro metadati e testi integrali
- `/.well-known/jwt-vc-issuer` — IETF (OAuth WG, draft stage). Dove un verificatore trova le chiavi di un emittente di credenziali verificabili
- `/.well-known/ai` — IETF draft (AI Discovery Endpoint). Una proposta di descrizione leggibile dalle macchine per agenti IA
- `_agent (DNS TXT record, no HTTP route)` — IETF draft (Agent Identity and Discovery, AID). Un record DNS che propone la scoperta dell'identità degli agenti
- `Content-Usage (robots.txt directive + HTTP header, no path)` — IETF AIPREF WG (draft-ietf-aipref-attach, WG-adopted, Standards Track). Una direttiva che dichiara cosa l'IA può fare con i contenuti
- `Schemamap (robots.txt directive; target URL free, conventionally /schema.txt)` — SCHEMA.TXT (specification on GitHub). Una direttiva che indica alle macchine la mappa degli schemi di un sito
- `/.well-known/did-configuration.json` — Decentralized Identity Foundation (DIF). Prova che collega un dominio a identificatori decentralizzati
- `_apertoid (DNS TXT record, no HTTP route)` — ApertoID (single vendor). Un record DNS di una proposta emergente di identità aperta
- `_x402 (DNS-TXT) + /.well-known/x402` — Individual draft (W. Hawkins) for the Coinbase/Cloudflare x402. Scoperta via DNS e web degli endpoint di pagamento x402
- `_agents / AIDISCA+AIINDEX (new DNS RR types)` — Verisign (individual draft). Tipi di record DNS proposti per la scoperta degli agenti
- `Link rel=client-ranges (HTTP Link header)` — Individual draft (Google/Ericsson authors). Un'intestazione che indica ai client gli intervalli IP dichiarati
- `Agentmap (robots.txt directive; target URL free)` — AI Catalog Working Group (Linux Foundation) — Agentic Resource Discovery spec. Una riga di robots.txt che indica alle macchine il catalogo di risorse IA di un sito
- `Archive-Embargo / Embargo-Allow (robots.txt directives, no path)` — Individual draft (M. Nottingham, M. Thomson — HTTP WG environment). Righe di robots.txt che regolano da quando le copie archiviate di un sito possono essere pubblicate
- `/agents.md` — Shopify (Plattform-Vorgabe) sowie die AGENTS.md-Konvention aus Code-Ablagen. Come un sito si descrive agli agenti IA
- `/.well-known/ucp` — Universal Commerce Protocol (UCP Tech Council). Quali funzioni di commercio un venditore offre agli agenti
- `/.well-known/agent-skills/index.json` — Cloudflare (Agent Skills Discovery RFC, Status Draft). Quali agent skill offre un dominio, con versione e checksum

_Le route osservate non vengono richieste nella misurazione mensile. Le nostre rilevazioni esplorative (vedi sotto) e una sonda mensile su 1.000 fonti del panel le richiedono, senza contarne nulla per questa pagina. Ogni voce ha il suo criterio di promozione nel lab._

### Richieste solo dalle rilevazioni esplorative (20)

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
**Che cosa richiediamo.** Gli elenchi qui sopra sono l'elenco completo delle
route che richiediamo: le route misurate in ogni misurazione mensile; le route
sotto osservazione solo nella sonda mensile su 1.000 fonti del panel e nelle
rilevazioni esplorative; le route sotto «Richieste solo dalle rilevazioni
esplorative» solo in quelle. Tre aggiunte: la vostra home page, una volta, per leggere i suoi annunci
`<link rel>` (la pagina stessa viene scartata); se i file del vostro stesso dominio
rimandano a un altro file lì — per esempio un link nel vostro `robots.txt` —
possiamo recuperare quel file una volta, al massimo un richiamo del genere per
dominio e per ciclo, con le stesse regole del `robots.txt`; e tre record DNS per
dominio (`_agent`, `_mcp`, `_index._agents`): semplici interrogazioni del
servizio dei nomi, che non toccano mai il vostro server web. Nulla di ciò che
recuperiamo viene pubblicato come contenuto — solo conteggi e quote per route,
e nulla in assoluto dalla sonda mensile o dalle rilevazioni esplorative.

**Come una route entra in tabella.** Le serve un editore identificabile oppure
un consumatore documentato che la legge — non basta che un formato circoli da
qualche parte. L'editore è indicato in tabella affinché ogni riga sia
verificabile da sé. Lo scopo dice che cosa fa il file su un server: lo
descrive, non lo giudica.

## Come misuriamo

La misurazione rispetta il vostro `robots.txt`, si identifica in modo onesto
indicando questo repository come mittente e procede lentamente e con parsimonia.
Vengono richiesti soltanto file di configurazione pubblici destinati alle
macchine — nessun contenuto delle pagine.

I valori qui sopra sono il **panel di ottobre 2026**: da ottobre 2026 un panel
stratificato di 10.000 fonti — un terzo del quadro di 30.000 — viene misurato
ogni mese; il panel precedente di 1.000 fonti prosegue al suo interno come
serie a sé (vedi le note sotto la tabella). Questa edizione non mostra la
freccia di tendenza; il perché è spiegato sotto la tabella. Ogni altra fonte
del quadro viene misurata una volta a trimestre. La **retrospettiva di 14 mesi** sulla diffusione delle
direttive AI annunciata per il primo rapporto mensile è pubblicata:
[REVIEW-2025-2026.md](REVIEW-2025-2026.md) — otto istantanee Common Crawl,
giugno 2025 – luglio 2026: intestazioni di risposta di **3,6 milioni di pagine**
(2,7 milioni di organizzazioni), più una scansione separata di oltre **270.000
file robots.txt**.

## File di dati al mese

La tabella qui sopra è il **panel**: 10.000 fonti fisse (un terzo del quadro),
misurate ogni mese. Solo panel contro panel può mostrare un cambiamento, e solo
all'interno di una serie: fino a dicembre 2026 il panel precedente di 1.000
fonti viene pubblicato accanto come serie a sé — l'unica che risale ad agosto
2026 — e le due serie non vengono mai concatenate. Ogni mese, nella stessa
misurazione, viene misurato anche un **blocco** del campione più ampio di
30.000 — suddiviso in tre blocchi (a, b, c) che ruotano nel trimestre, così
ogni fonte di blocco viene visitata una volta per trimestre. Il blocco **b** è
stato misurato a ottobre 2026. Lo scopo della misurazione di blocco è la
copertura, non la tendenza.

Tutte le serie sono in [`data/`](data/): `panel-AAAA-MM.{json,csv}`,
`panel1000-AAAA-MM.{json,csv}` e `monat-AAAA-MM-block-x.{json,csv}`. Ogni file dichiara da sé quando è
stato misurato e se è completo (`measurement_window.status`); come viene
suddiviso il campione è definito in [RULESET.md](RULESET.md).

## Chi c'è dietro

Il radar è gestito da **Berger+Team**, un collettivo di freelance altoatesino,
accanto al lavoro su [btlabs Core](https://btlabs.dev/it). La misurazione nasce
perché quel lavoro ha bisogno di numeri anziché di supposizioni: quali percorsi
di discovery vengono davvero usati e di quali si parla soltanto. Viene
pubblicato ciò che è stato misurato — comprese le rotte risultate a zero.

## Come escludersi

Nessuna domanda, nessuna motivazione necessaria. Basta una di queste vie:

1. una e-mail a **florian@berger.team** con il dominio — per questa via
   non serve un account GitHub, **oppure**
2. una issue in questo repository con il dominio, **oppure**
3. una regola `Disallow` per il nostro identificativo `ai-discovery-radar` nel vostro `robots.txt` —
   funziona senza alcun contatto.

I domini esclusi vengono saltati **prima** che venga inviata qualsiasi richiesta.
Contatti, correzioni e l'impegno completo: [SECURITY.md](SECURITY.md).

## Attribuzione del campione

Il campione di domini è estratto dalla [lista Tranco](https://tranco-list.eu/)
(classifica per la ricerca; il nostro quadro congelato fa riferimento a un ID
permanente di lista Tranco) e dalle
[top list del Chrome UX Report](https://github.com/zakird/crux-top-lists)
(© Google, [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)).
Tranco stessa aggrega diverse fonti, tra cui la Majestic Million
(© Majestic, [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/)).

## Licenza

MIT — vedi [LICENSE](LICENSE).
