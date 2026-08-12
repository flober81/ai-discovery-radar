# ai-discovery-radar

[English](README.md) · [Deutsch](README.de.md) · **Italiano**

> **Trovato questo identificativo nei log del vostro server?** Potete escludervi
> con una sola riga — vedi [Come escludersi](#come-escludersi). Nessun account,
> nessun contatto, nessuna motivazione richiesta.

Un radar dei file di AI discovery sul web pubblico: quali route esistono
(`robots.txt`, `llms.txt`, `ai-catalog.json`, …), quanto sono diffuse e se sono
davvero scaricabili. Ogni segnale è una misurazione, non un'opinione. Con quale
cadenza si misura verrà indicato qui non appena ci saranno misurazioni a
dimostrarlo.

## Il radar

<!-- RADAR:START -->
_34 route nel catalogo · nessuna misurazione pubblicata_

| Route | Scopo | Editore | Diffusione |
|:--|:--|:--|--:|
| `/robots.txt` | Quali aree di un sito i crawler possono visitare | IETF | — |
| `/sitemap.xml` | L'elenco di tutti gli indirizzi che un sito offre | sitemaps.org | — |
| `/.well-known/security.txt` | Dove segnalare una vulnerabilità di sicurezza | IETF | — |
| `/security.txt` | Dove segnalare una vulnerabilità, alla radice del sito | IETF | — |
| `/.well-known/api-catalog` | L'elenco delle interfacce offerte da un dominio | IETF | — |
| `/.well-known/tdmrep.json` | Se testi e dati possono essere estratti automaticamente | W3C TDM Reservation Protocol CG | — |
| `/.well-known/gpc.json` | Se il sito rispetta l'opt-out sulla condivisione dei dati | W3C Global Privacy Control | — |
| `/.well-known/dnt-policy.txt` | La promessa di non tracciare i visitatori tra i siti | EFF | — |
| `/.well-known/host-meta` | I rimandi agli altri punti informativi di un dominio | IETF | — |
| `/.well-known/webfinger` | Chi sta dietro un indirizzo di questo dominio | IETF | — |
| `/.well-known/oauth-protected-resource` | Dove un client ottiene l'autorizzazione all'accesso | IETF | — |
| `/.well-known/oauth-authorization-server` | Come funziona il servizio che concede l'accesso | IETF | — |
| `/.well-known/openid-configuration` | Dove e come si accede a questo dominio | OpenID Foundation | — |
| `/.well-known/openid-federation` | A quale federazione appartiene un soggetto, con prova | OpenID Foundation | — |
| `/.well-known/traffic-advice` | Se un proxy di cache può precaricare le pagine | Google (Private Prefetch Proxy) | — |
| `/.well-known/ai-catalog.json` | Quali contenuti e servizi un dominio offre agli agenti AI | AI Catalog WG (Linux Foundation), Google, Microsoft | — |
| `/.well-known/agent-card.json` | Cosa sa fare un agente software e come interpellarlo | A2A Project (Linux Foundation) | — |
| `/.well-known/agent.json` | Le capacità di un agente, col vecchio nome di file | A2A Project (Linux Foundation) | — |
| `/.well-known/mcp.json` | Quali tool server un dominio mette a disposizione per AI | Model Context Protocol | — |
| `/.well-known/mcp-server` | Dove raggiungere il tool server di un dominio | IETF (individual draft) | — |
| `/openapi.json` | La descrizione di un'interfaccia per altri programmi | OpenAPI Initiative | — |
| `/.well-known/openapi.json` | La descrizione dell'interfaccia nella cartella well-known | OpenAPI Initiative | — |
| `/.well-known/x402.json` | Prezzo e modo di pagamento per le richieste automatiche | Coinbase, Cloudflare | — |
| `/.well-known/did.json` | L'identità verificabile di un dominio senza enti centrali | W3C | — |
| `/llms.txt` | Un indice dei contenuti per i modelli linguistici | Answer.AI | — |
| `/llms-full.txt` | L'intero contenuto di un sito in un unico file | Answer.AI | — |
| `/ai.txt` | Quali contenuti sono esclusi dall'addestramento di AI | Spawning | — |
| `/.well-known/ai.txt` | Le stesse regole d'uso per AI nella cartella well-known | Spawning | — |
| `/swagger.json` | La descrizione dell'interfaccia col vecchio nome di file | SmartBear (Swagger) | — |
| `/rsl.xml` | A quali condizioni di licenza si possono usare i contenuti | RSL Collective | — |
| `/humans.txt` | Chi ha realizzato un sito, in forma leggibile | humanstxt.org | — |
| `/.well-known/ai-plugin.json` | Istruzioni perché un chatbot possa usare un servizio | OpenAI | — |
| `/ai-plugin.json` | Le stesse istruzioni per chatbot, alla radice del sito | OpenAI | — |
| `/.well-known/llms.txt` | Un indice per i modelli linguistici, in well-known | Answer.AI | — |

I dati di diffusione compariranno con la prima misurazione pubblicata.

<!-- RADAR:END -->
Questa tabella è completa: elenca ogni route che richiediamo, e ciò che non
compare qui non lo richiediamo. Una route entra in elenco quando ha un editore
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

Il campione di domini proviene dalla Majestic Million
(© Majestic, [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/)).

## Licenza

MIT — vedi [LICENSE](LICENSE).
