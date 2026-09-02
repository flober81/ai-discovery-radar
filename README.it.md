# ai-discovery-radar

[English](README.md) · [Deutsch](README.de.md) · **Italiano**

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22178282.svg)](https://doi.org/10.5281/zenodo.22178282)

> **Trovato questo identificativo nei log del vostro server?** Potete escludervi
> con una sola riga — vedi [Come escludersi](#come-escludersi). Nessun account,
> nessun contatto, nessuna motivazione richiesta.
>
> **Quanto spesso passiamo:** circa **10.700 fonti (domini) al mese** — una
> parte a rotazione del quadro di ~30.000 fonti, ognuna di queste al massimo
> una volta a trimestre, più una piccola parte fissa che rivisitiamo ogni mese,
> così il cambiamento da un mese all'altro diventa misurabile.

Un radar dei file di AI discovery sul web pubblico: quali route esistono
(`robots.txt`, `llms.txt`, `ai-catalog.json`, …), quanto sono diffuse e se sono
davvero scaricabili. Ogni segnale è una misurazione, non un'opinione.

## Il radar

<!-- RADAR:START -->
_Misurazione **panel-2026-08** · 853 host raggiungibili (853 domini registrabili) · regole 0.3.1_

| Route | Scopo | Editore | n | Diffusione | IC 95 % | Tendenza |
|:--|:--|:--|--:|--:|:--|:-:|
| `/robots.txt` | Quali aree di un sito i crawler possono visitare | IETF | 760 | 86,45 % | 83,8–88,7 | — |
| `/sitemap.xml` | L'elenco di tutti gli indirizzi che un sito offre | sitemaps.org | 680 | 54,56 % | 50,8–58,3 | — |
| `/llms.txt` | Un indice dei contenuti per i modelli linguistici | Answer.AI | 662 | 12,99 % | 10,6–15,8 | — |
| `/.well-known/security.txt` | Dove segnalare una vulnerabilità di sicurezza | IETF | 681 | 6,75 % | 5,1–8,9 | — |
| `/.well-known/oauth-authorization-server` | Come funziona il servizio che concede l'accesso | IETF | 675 | 5,19 % | 3,8–7,1 | — |
| `/llms-full.txt` | L'intero contenuto di un sito in un unico file | Answer.AI | 665 | 4,66 % | 3,3–6,5 | — |
| `/.well-known/oauth-protected-resource` | Dove un client ottiene l'autorizzazione all'accesso | IETF | 676 | 4,59 % | 3,2–6,4 | — |
| `/.well-known/gpc.json` | Se il sito rispetta l'opt-out sulla condivisione dei dati | W3C Global Privacy Control | 677 | 2,81 % | 1,8–4,3 | — |
| `/humans.txt` | Chi ha realizzato un sito, in forma leggibile | humanstxt.org | 662 | 1,66 % | 0,9–3,0 | — |
| `/.well-known/traffic-advice` | Se un proxy di cache può precaricare le pagine | Google (Private Prefetch Proxy) | 673 | 1,34 % | 0,7–2,5 | — |
| `/security.txt` | Dove segnalare una vulnerabilità, alla radice del sito | IETF | 696 | 1,15 % | 0,6–2,3 | — |
| `/rsl.xml` | A quali condizioni di licenza si possono usare i contenuti | RSL Collective | 640 | 0,78 % | 0,3–1,8 | — |
| `/ai.txt` | Quali contenuti sono esclusi dall'addestramento di AI | Spawning | 667 | 0,45 % | 0,2–1,3 | — |
| `/.well-known/tdmrep.json` | Se testi e dati possono essere estratti automaticamente | W3C TDM Reservation Protocol CG | 678 | 0,29 % | 0,1–1,1 | — |
| `/.well-known/api-catalog` | L'elenco delle interfacce offerte da un dominio | IETF | 678 | 0,15 % | 0,0–0,8 | — |
| `/.well-known/mcp.json` | Quali tool server un dominio mette a disposizione per AI | Model Context Protocol | 674 | 0,15 % | 0,0–0,8 | — |
| `/.well-known/openid-configuration` | Dove e come si accede a questo dominio | OpenID Foundation | 674 | 0,15 % | 0,0–0,8 | — |
| `/openapi.json` | La descrizione di un'interfaccia per altri programmi | OpenAPI Initiative | 650 | 0,15 % | 0,0–0,9 | — |
| `/.well-known/agent-card.json` | Cosa sa fare un agente software e come interpellarlo | A2A Project (Linux Foundation) | 672 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/agent.json` | Le capacità di un agente, col vecchio nome di file | A2A Project (Linux Foundation) | 672 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/ai-catalog.json` | Quali contenuti e servizi un dominio offre agli agenti AI | AI Catalog WG (Linux Foundation), Google, Microsoft | 671 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/ai-plugin.json` | Istruzioni perché un chatbot possa usare un servizio | OpenAI | 656 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/ai.txt` | Le stesse regole d'uso per AI nella cartella well-known | Spawning | 661 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/did.json` | L'identità verificabile di un dominio senza enti centrali | W3C | 672 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/dnt-policy.txt` | La promessa di non tracciare i visitatori tra i siti | EFF | 678 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/host-meta` | I rimandi agli altri punti informativi di un dominio | IETF | 670 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/llms.txt` | Un indice per i modelli linguistici, in well-known | Answer.AI | 658 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/mcp-server` | Dove raggiungere il tool server di un dominio | IETF (individual draft) | 673 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/openapi.json` | La descrizione dell'interfaccia nella cartella well-known | OpenAPI Initiative | 673 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/openid-federation` | A quale federazione appartiene un soggetto, con prova | OpenID Foundation | 677 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/webfinger` | Chi sta dietro un indirizzo di questo dominio | IETF | 671 | 0,00 % | 0,0–0,6 | — |
| `/.well-known/x402.json` | Prezzo e modo di pagamento per le richieste automatiche | Coinbase, Cloudflare | 670 | 0,00 % | 0,0–0,6 | — |
| `/ai-plugin.json` | Le stesse istruzioni per chatbot, alla radice del sito | OpenAI | 641 | 0,00 % | 0,0–0,6 | — |
| `/swagger.json` | La descrizione dell'interfaccia col vecchio nome di file | SmartBear (Swagger) | 642 | 0,00 % | 0,0–0,6 | — |

La diffusione è la quota delle fonti che abbiamo potuto davvero consultare
e che hanno restituito la route, con intervallo di Wilson al 95 %. Le fonti
che ci hanno respinto (bot wall), che vietano il prelievo via robots.txt o
che non erano raggiungibili vengono contate e riportate a parte — ma una
non-risposta non è un «no», quindi non entra nel denominatore.
**`n` è il numero di host su cui la route è stata effettivamente testata.
Cambia da una route all'altra, quindi ogni riga ha il proprio denominatore
e le righe non sono direttamente confrontabili tra loro.**
Non c'è ancora una misurazione precedente con cui confrontare.



## Sotto osservazione (18)

**Confermate** — registrate (IANA) o RFC, quasi assenti sul campo:

- `/.well-known/nostr.json` — Nostr Developer Community (NIP-05). Prova che una chiave pubblica appartiene a un nome di questo dominio
- `/.well-known/vacation-rental.json` — Vacation Rental Protocol (single registrant). Documento di scoperta per offerte di soggiorno firmate crittograficamente
- `/.well-known/xregistry` — xRegistry Authors (CNCF Sandbox). Punto d'ingresso di un registro estensibile per schemi ed eventi
- `/.well-known/host-meta.json` — IETF. Il gemello JSON dei rimandi host-meta

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

_Osservato significa osservato: nulla di ciò è misurato o conteggiato sopra. Ogni voce ha il suo criterio di promozione nel lab._
<!-- RADAR:END -->
**Che cosa richiediamo.** La tabella qui sopra è l'elenco completo delle route
che richiediamo regolarmente. Due aggiunte: se i file del vostro stesso dominio
rimandano a un altro file lì — per esempio un link nel vostro `robots.txt` —
possiamo recuperare quel file una volta, al massimo un richiamo del genere per
dominio e per ciclo, con le stesse regole del `robots.txt`. E consultiamo tre
record DNS per dominio (`_agent`, `_mcp`, `_index._agents`): semplici
interrogazioni del servizio dei nomi, che non toccano mai il vostro server web.

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

I valori qui sopra sono la **base di agosto 2026**: un panel stratificato di
1.000 fonti, misurato una volta. Da **settembre 2026** il panel viene misurato
ogni mese, e ogni fonte del campione più ampio una volta a trimestre. Insieme
al primo rapporto mensile verrà pubblicata anche una **retrospettiva di 14
mesi** sulla diffusione delle direttive AI (giugno 2025 – luglio 2026), basata
su oltre **270.000 file robots.txt analizzati**.

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
3. una regola `Disallow` per il nostro identificativo nel vostro `robots.txt` —
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
