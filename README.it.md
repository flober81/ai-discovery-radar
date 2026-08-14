# ai-discovery-radar

[English](README.md) · [Deutsch](README.de.md) · **Italiano**

> **Trovato questo identificativo nei log del vostro server?** Potete escludervi
> con una sola riga — vedi [Come escludersi](#come-escludersi). Nessun account,
> nessun contatto, nessuna motivazione richiesta.

Un radar dei file di AI discovery sul web pubblico: quali route esistono
(`robots.txt`, `llms.txt`, `ai-catalog.json`, …), quanto sono diffuse e se sono
davvero scaricabili. Ogni segnale è una misurazione, non un'opinione. La
tabella sotto mostra la **base di agosto 2026**: un panel stratificato di
1.000 domini, misurato una volta. Da **settembre 2026** il panel viene
misurato ogni mese, e ogni dominio del campione più ampio una volta a
trimestre.

## Il radar

<!-- RADAR:START -->
_Misurazione **panel-2026-08** · 853 host raggiungibili (853 domini registrabili) · regole 0.2.0_

| Route | Scopo | Editore | n | Diffusione | IC 95 % | Tendenza |
|:--|:--|:--|--:|--:|:--|:-:|
| `/robots.txt` | Quali aree di un sito i crawler possono visitare | IETF | 853 | 77,02 % | 74,1–79,7 | — |
| `/sitemap.xml` | L'elenco di tutti gli indirizzi che un sito offre | sitemaps.org | 842 | 44,06 % | 40,7–47,4 | — |
| `/llms.txt` | Un indice dei contenuti per i modelli linguistici | Answer.AI | 842 | 10,21 % | 8,3–12,4 | — |
| `/.well-known/security.txt` | Dove segnalare una vulnerabilità di sicurezza | IETF | 842 | 5,46 % | 4,1–7,2 | — |
| `/.well-known/oauth-authorization-server` | Come funziona il servizio che concede l'accesso | IETF | 842 | 4,16 % | 3,0–5,7 | — |
| `/.well-known/oauth-protected-resource` | Dove un client ottiene l'autorizzazione all'accesso | IETF | 842 | 3,68 % | 2,6–5,2 | — |
| `/llms-full.txt` | L'intero contenuto di un sito in un unico file | Answer.AI | 842 | 3,68 % | 2,6–5,2 | — |
| `/.well-known/gpc.json` | Se il sito rispetta l'opt-out sulla condivisione dei dati | W3C Global Privacy Control | 842 | 2,26 % | 1,4–3,5 | — |
| `/humans.txt` | Chi ha realizzato un sito, in forma leggibile | humanstxt.org | 842 | 1,31 % | 0,7–2,3 | — |
| `/.well-known/traffic-advice` | Se un proxy di cache può precaricare le pagine | Google (Private Prefetch Proxy) | 842 | 1,07 % | 0,6–2,0 | — |
| `/security.txt` | Dove segnalare una vulnerabilità, alla radice del sito | IETF | 842 | 0,95 % | 0,5–1,9 | — |
| `/rsl.xml` | A quali condizioni di licenza si possono usare i contenuti | RSL Collective | 842 | 0,59 % | 0,3–1,4 | — |
| `/ai.txt` | Quali contenuti sono esclusi dall'addestramento di AI | Spawning | 842 | 0,36 % | 0,1–1,0 | — |
| `/.well-known/tdmrep.json` | Se testi e dati possono essere estratti automaticamente | W3C TDM Reservation Protocol CG | 842 | 0,24 % | 0,1–0,9 | — |
| `/.well-known/api-catalog` | L'elenco delle interfacce offerte da un dominio | IETF | 842 | 0,12 % | 0,0–0,7 | — |
| `/.well-known/mcp.json` | Quali tool server un dominio mette a disposizione per AI | Model Context Protocol | 842 | 0,12 % | 0,0–0,7 | — |
| `/.well-known/openid-configuration` | Dove e come si accede a questo dominio | OpenID Foundation | 842 | 0,12 % | 0,0–0,7 | — |
| `/openapi.json` | La descrizione di un'interfaccia per altri programmi | OpenAPI Initiative | 842 | 0,12 % | 0,0–0,7 | — |
| `/.well-known/agent-card.json` | Cosa sa fare un agente software e come interpellarlo | A2A Project (Linux Foundation) | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/agent.json` | Le capacità di un agente, col vecchio nome di file | A2A Project (Linux Foundation) | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/ai-catalog.json` | Quali contenuti e servizi un dominio offre agli agenti AI | AI Catalog WG (Linux Foundation), Google, Microsoft | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/ai-plugin.json` | Istruzioni perché un chatbot possa usare un servizio | OpenAI | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/ai.txt` | Le stesse regole d'uso per AI nella cartella well-known | Spawning | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/did.json` | L'identità verificabile di un dominio senza enti centrali | W3C | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/dnt-policy.txt` | La promessa di non tracciare i visitatori tra i siti | EFF | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/host-meta` | I rimandi agli altri punti informativi di un dominio | IETF | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/llms.txt` | Un indice per i modelli linguistici, in well-known | Answer.AI | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/mcp-server` | Dove raggiungere il tool server di un dominio | IETF (individual draft) | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/openapi.json` | La descrizione dell'interfaccia nella cartella well-known | OpenAPI Initiative | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/openid-federation` | A quale federazione appartiene un soggetto, con prova | OpenID Foundation | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/webfinger` | Chi sta dietro un indirizzo di questo dominio | IETF | 842 | 0,00 % | 0,0–0,5 | — |
| `/.well-known/x402.json` | Prezzo e modo di pagamento per le richieste automatiche | Coinbase, Cloudflare | 842 | 0,00 % | 0,0–0,5 | — |
| `/ai-plugin.json` | Le stesse istruzioni per chatbot, alla radice del sito | OpenAI | 842 | 0,00 % | 0,0–0,5 | — |
| `/swagger.json` | La descrizione dell'interfaccia col vecchio nome di file | SmartBear (Swagger) | 842 | 0,00 % | 0,0–0,5 | — |

La diffusione è la quota di host raggiungibili che hanno restituito la route,
con intervallo di Wilson al 95 %. Ogni valore è un limite inferiore dal punto
di vista di un agente non privilegiato: un file che esiste ma non può essere
scaricato non viene contato.
**`n` è il numero di host su cui la route è stata effettivamente testata.
Cambia da una route all'altra, quindi ogni riga ha il proprio denominatore
e le righe non sono direttamente confrontabili tra loro.**
Non c'è ancora una misurazione precedente con cui confrontare.

<!-- RADAR:END -->
Questa tabella è l'elenco completo delle route che richiediamo regolarmente.
Un'aggiunta: se i file del vostro stesso dominio rimandano a un altro file
lì (per esempio un link nel vostro `robots.txt`), possiamo recuperare quel
file una volta — al massimo un simile richiamo per dominio e per ciclo, con
le stesse regole del `robots.txt`. Inoltre consultiamo tre record DNS per
dominio (`_agent`, `_mcp`, `_index._agents`) — semplici interrogazioni del
servizio dei nomi che non toccano mai il vostro server web.
Una route entra in elenco quando ha un editore
identificabile oppure un consumatore documentato che la legge — non perché un
formato circoli da qualche parte. L'editore è indicato in tabella affinché ogni
riga sia verificabile da sé. Lo scopo dice che cosa fa il file su un server: lo
descrive, non lo giudica.

## Come misuriamo

La misurazione rispetta il vostro `robots.txt`, si identifica in modo onesto
indicando questo repository come mittente e procede lentamente e con parsimonia.
Vengono richiesti soltanto file di configurazione pubblici destinati alle
macchine — nessun contenuto delle pagine.

## Come escludersi

Nessuna domanda, nessuna motivazione necessaria. Basta una di queste vie:

1. una e-mail a **florian.f.berger@gmail.com** con il dominio — per questa via
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
