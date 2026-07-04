# Sebastians Skill Repo

Sechs Claude Skills aus der Produkt-Praxis: Positionierung, UX-Audits, Linear-Tickets, Ideen-Validierung, Bewerbungs-Checks und Schreiben, das nicht nach AI klingt.

## Wer dahinter steckt

Ich bin [Sebastian Lohrmann](https://sebastian-lohrmann.de), Data Driven Product Lead. Menschen in ihrer Arbeit erfolgreich zu machen, ist mein Antrieb. Von Startup bis Konzern führe ich agile Teams mit einem kollaborativen und datengetriebenen Ansatz zu Top Outcomes. Mein technisches Verständnis erlaubt es mir, fliessend Developer zu sprechen und zwischen allen Stakeholdern zu vermitteln. Als Product Designer gestalte ich Experiences, die schön und intuitiv zugleich sind.

Diese Skills sind Werkzeuge aus genau dieser Arbeit. Jeder einzelne kodiert einen Prozess, den ich sonst von Hand durchlaufen würde: ein Framework, einen Qualitätsstandard, eine Methode. Claude wendet sie an, ich behalte die Kontrolle über das Ergebnis.

## Was ist ein Skill?

Ein Skill ist eine strukturierte Arbeitsanweisung für Claude. Jede `.skill`-Datei ist ein Zip-Archiv mit einer `SKILL.md` (plus Referenzdateien), die Claude sagt, wann und wie ein bestimmter Prozess abläuft. Einmal installiert, erkennt Claude selbst, wann ein Skill passt. Du musst ihn nicht explizit aufrufen.

## Installation

**Claude (Web und Desktop):** Einstellungen → Fähigkeiten → Skill hochladen, dann die gewünschte `.skill`-Datei auswählen.

**Claude Code:** Die `.skill`-Datei ist ein Zip. Entpacken und den Ordner nach `~/.claude/skills/` legen:

```bash
unzip ux-audit.skill -d ~/.claude/skills/
```

## Die Skills

### anti-ai-writing

Erzwingt Texte, die nach Mensch klingen statt nach ChatGPT. Basiert auf dem Katalog von Wikipedias WikiProject AI Cleanup: keine Gedankenstriche, kein "Das ist kein X, das ist Y", keine Buzzwords, keine aufgeblasene Bedeutung. Funktioniert auf Deutsch und Englisch.

**Einsatz:** Bei jedem Schreib-Task aktiv lassen. Oder direkt anstossen: *"Schreib mir den LinkedIn-Post, aber bitte so, dass er nicht nach AI klingt."*

### b2b-positioning

Entwickelt B2B-Positionierung nach der Methode von April Dunford: Competitive Alternatives, Differentiated Capabilities, Differentiated Value, Best-Fit Customers, Market Category. In genau dieser Reihenfolge, weil jede Komponente auf der vorherigen aufbaut. Enthält auch eine Anleitung für Positioning-Workshops.

**Einsatz:** *"Hilf mir, die Positionierung für unser Produkt zu schärfen"* oder wenn du an Landing Pages, Pitch Decks oder Messaging arbeitest und die Frage "für wen und warum wir?" noch offen ist.

### job-application-match

Bewertet, wie gut eine Bewerbung (CV plus Anschreiben) auf eine konkrete Stellenanzeige passt. Fünf Phasen: Intake, JD-Decoding, Bewerbungs-Decoding, Matching mit Begründung, Report mit konkreten Empfehlungen. Zweisprachig (DE/EN) mit automatischer Spracherkennung.

**Einsatz:** Stellenanzeige und CV in den Chat werfen und fragen: *"Passt mein CV auf diese Stelle?"* oder *"Soll ich mich bewerben?"*

### linear-tickets

Schreibt strukturierte, halluzinationsfreie Linear-Tickets. Harte Regel: Interview vor Ticket. Der Skill fragt erst nach, was unklar ist, statt Anforderungen zu halluzinieren. Die Ticketsprache leitet er aus den bestehenden Tickets des Projekts ab.

**Einsatz:** *"Schreib ein Ticket für..."*, *"Brich das Feature in Issues runter"* oder eine Anforderung beschreiben, die ins Backlog soll.

### proven-better-new

Validiert Produktideen mit Mark Pincus' "Proven, Better, New"-Framework (aus "Life at the Speed of Play", 2026). Erst Interview, dann Scoring gegen die Rubrik, am Ende ein klares Verdikt: BUILD, TEST FIRST, REWORK oder KILL THE IDEA, KEEP THE INSTINCT. Zweisprachig (DE/EN).

**Einsatz:** *"Validiere diese Produktidee"*, *"Sollten wir das bauen?"* oder eine Idee beschreiben und nach dem PBN-Score fragen.

### ux-audit

Führt einen strukturierten UX-Audit durch: auf Screenshots, Figma-Dateien, Live-URLs oder Recordings. Standard ist das Vollaudit mit Heuristik-Pass, Bias- und Prinzip-Linsen sowie Accessibility-Check, priorisiert nach Severity. Für den schnellen Blick gibt es den Quick-Scan.

**Einsatz:** Screenshots oder Figma-Link posten und fragen: *"Mach einen UX-Audit"* oder *"Wo verlieren wir Nutzer in diesem Flow?"* Für die kurze Variante: *"Schau kurz drüber."*

## Lizenz und Nutzung

Nimm, was du brauchst, und pass es an deinen Kontext an. Die Skills sind bewusst als editierbare Markdown-Dateien gebaut: entpacken, `SKILL.md` anpassen, wieder zippen, fertig.
