# Contact, opt-out and corrections

**English** · [Deutsch](#deutsch) · [Italiano](#italiano)

This file carries all three languages in full. The way out is the point of the
document, so nobody should have to follow a link to find it in their own
language.

## English

### If you landed here because our crawler visited you

The user agent `ai-discovery-radar/…` belongs to a research project that measures which
machine-readable discovery files exist on the web and whether AI agents can fetch them at
all. Only public configuration files are requested (`robots.txt`, `llms.txt`,
`security.txt`, `ai-catalog.json` and the like) — no page content, no APIs, no personal
data.

**How we behave:**

- Your `robots.txt` first, evaluated for our own token. Whatever it forbids us, we do
  **not** fetch.
- We identify ourselves honestly and **never** pose as another bot. The requests come from
  one fixed address that explains itself: http://145.223.96.128
- One request at a time per host, a pause in between — **at least as long as a
  `Crawl-delay` in your `robots.txt` asks for** — backoff on 429/503, and we stop
  after six rejections. Your site sees a few dozen requests per measurement run — one per
  route from the table in the [README](README.md). That table is the complete list —
  whatever is not in it, we do not request.
- We publish observations, not assessments — we do not hand out grades.

### Opt out

No questions asked, no reason needed: (1) an email to **florian.f.berger@gmail.com** with
the domain, (2) an issue in this repository with the domain, or (3) a `Disallow` rule for
our token in your `robots.txt`. For (1) you do not need a GitHub account. Excluded domains
are skipped **before** any request is made.

### Something wrong with our figures?

A published number is incorrect? Email or issue — we correct it and document the
correction.

### Security vulnerabilities in this project

Please report these through this repository's GitHub Security Advisories, not through a
public issue.

---

## Deutsch

### Wenn Sie hier gelandet sind, weil unser Crawler Sie besucht hat

Der User-Agent `ai-discovery-radar/…` gehört zu einem Forschungsprojekt, das misst, welche
maschinenlesbaren Discovery-Dateien im Web existieren und ob sie für KI-Agenten abrufbar sind.
Abgerufen werden ausschließlich öffentliche Konfigurationsdateien (`robots.txt`, `llms.txt`,
`security.txt`, `ai-catalog.json` und ähnliche) — keine Seiteninhalte, keine APIs, keine
personenbezogenen Daten.

**Wie wir uns verhalten:**

- Zuerst Ihre `robots.txt`, ausgewertet für unser eigenes Token. Was dort für uns gesperrt ist,
  rufen wir **nicht** ab.
- Wir geben uns ehrlich zu erkennen und **niemals** als ein anderer Bot aus. Die Abrufe kommen
  von einer festen Adresse, die sich selbst erklärt: http://145.223.96.128
- Eine Anfrage zur Zeit pro Host, Pause dazwischen — **mindestens so lang, wie ein
  `Crawl-delay` in Ihrer `robots.txt` es wünscht** — Backoff bei 429/503, Abbruch nach sechs
  Abweisungen. Ihre Seite sieht wenige Dutzend Anfragen pro Messlauf — je eine je Route aus der
  Tabelle in der [README](README.de.md). Diese Tabelle ist die vollständige Liste — was dort
  nicht steht, rufen wir nicht ab.
- Wir veröffentlichen Beobachtungen, keine Bewertungen — eine Note vergeben wir nicht.

### Austragung

Keine Rückfragen, keine Begründung nötig: (1) E-Mail an **florian.f.berger@gmail.com** mit der
Domain, (2) ein Issue in diesem Repository mit der Domain oder (3) `Disallow` für unser Token in
Ihrer `robots.txt`. Für Weg 1 brauchen Sie kein GitHub-Konto. Ausgetragene Domains werden **vor**
dem Abruf übersprungen.

### Fehler in unseren Zahlen

Eine veröffentlichte Zahl ist falsch? E-Mail oder Issue — wir korrigieren und dokumentieren die
Korrektur.

### Sicherheitslücken in diesem Projekt

Bitte über die GitHub Security Advisories dieses Repositories melden, nicht über ein
öffentliches Issue.

---

## Italiano

### Se siete arrivati qui perché il nostro crawler ha visitato il vostro sito

Lo user agent `ai-discovery-radar/…` appartiene a un progetto di ricerca che misura quali
file di discovery leggibili dalle macchine esistono sul web e se gli agenti AI riescano
davvero a scaricarli. Vengono richiesti soltanto file di configurazione pubblici
(`robots.txt`, `llms.txt`, `security.txt`, `ai-catalog.json` e simili) — nessun contenuto
delle pagine, nessuna API, nessun dato personale.

**Come ci comportiamo:**

- Prima di tutto il vostro `robots.txt`, interpretato per il nostro identificativo. Ciò che
  ci viene vietato lì **non** lo richiediamo.
- Ci identifichiamo in modo onesto e **mai** ci spacciamo per un altro bot. Le richieste
  arrivano da un unico indirizzo fisso che si spiega da sé: http://145.223.96.128
- Una richiesta alla volta per host, con pausa tra una e l'altra — **lunga almeno quanto
  chiede un `Crawl-delay` nel vostro `robots.txt`** — backoff su 429/503 e
  interruzione dopo sei rifiuti. Il vostro sito riceve poche decine di richieste per
  misurazione — una per ogni route della tabella nella [README](README.it.md). Quella
  tabella è l'elenco completo: ciò che non compare lì, non lo richiediamo.
- Pubblichiamo osservazioni, non valutazioni — non assegniamo voti.

### Come escludersi

Nessuna domanda, nessuna motivazione necessaria: (1) una e-mail a
**florian.f.berger@gmail.com** con il dominio, (2) una issue in questo repository con il
dominio oppure (3) una regola `Disallow` per il nostro identificativo nel vostro
`robots.txt`. Per la prima via non serve un account GitHub. I domini esclusi vengono
saltati **prima** che venga inviata qualsiasi richiesta.

### Errori nei nostri dati

Un dato pubblicato è sbagliato? E-mail o issue — lo correggiamo e documentiamo la
correzione.

### Vulnerabilità di sicurezza in questo progetto

Segnalatele tramite i GitHub Security Advisories di questo repository, non con una issue
pubblica.
