# Kontakt, Austragung, Meldungen

## Wenn Sie hier gelandet sind, weil unser Crawler Sie besucht hat

Der User-Agent `ai-discovery-radar/…` gehört zu einem Forschungsprojekt, das misst, welche
maschinenlesbaren Discovery-Dateien im Web existieren und ob sie für KI-Agenten abrufbar sind.
Abgerufen werden ausschließlich öffentliche Konfigurationsdateien (`robots.txt`, `llms.txt`,
`security.txt`, `ai-catalog.json` und ähnliche) — keine Seiteninhalte, keine APIs, keine
personenbezogenen Daten.

**Wie wir uns verhalten:**

- Zuerst Ihre `robots.txt`, ausgewertet für unser eigenes Token. Was dort für uns gesperrt ist,
  rufen wir **nicht** ab.
- Wir geben uns ehrlich zu erkennen und **niemals** als ein anderer Bot aus.
- Eine Anfrage zur Zeit pro Host, Pause dazwischen, Backoff bei 429/503, Abbruch nach sechs
  Abweisungen. Ihre Seite sieht wenige Dutzend Anfragen pro Messlauf — je eine je Route aus der
  Tabelle in der [README](README.md). Diese Tabelle ist die vollständige Liste — was dort
  nicht steht, rufen wir nicht ab.
- Wir veröffentlichen Beobachtungen, keine Bewertungen — eine Note vergeben wir nicht.

## Austragung

Keine Rückfragen, keine Begründung nötig: (1) E-Mail an **florian.f.berger@gmail.com** mit der
Domain, (2) ein Issue in diesem Repository mit der Domain oder (3) `Disallow` für unser Token in
Ihrer `robots.txt`. Für Weg 1 brauchen Sie kein GitHub-Konto. Ausgetragene Domains werden **vor**
dem Abruf übersprungen.

## Fehler in unseren Zahlen

Eine veröffentlichte Zahl ist falsch? E-Mail oder Issue — wir korrigieren und dokumentieren die
Korrektur.

## Sicherheitslücken in diesem Projekt

Bitte über die GitHub Security Advisories dieses Repositories melden, nicht über ein
öffentliches Issue.

## Opt-out (English)

Don't want your domain measured? No questions asked:

1. An email to **florian.f.berger@gmail.com** with the domain, **or**
2. an issue in this repository with the domain, **or**
3. a `Disallow` rule for our token in your `robots.txt`.

Excluded domains are skipped before any request is made.
