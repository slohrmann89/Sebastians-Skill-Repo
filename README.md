# Sebastians Skill Repo

Sieben Claude Skills aus der Produkt-Praxis: Positionierung für Produkte und Personen, UX-Audits, Linear-Tickets, Ideen-Validierung, Bewerbungs-Checks und Schreiben, das nicht nach AI klingt.

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

### personal-brand-positioning

Entwickelt eine tragfähige Personal-Brand-Positionierung per strukturiertem Interview. Kombiniert Rebecca Okamotos "20 Words or Less" mit April Dunfords Komponenten (adaptiert für Personen), David Perells Personal Monopoly, Naval Ravikants Specific Knowledge und Wes Kaos Spiky Point of View. Erster Output ist ein One-Liner in maximal 20 Wörtern ("Ich helfe X, Y zu erreichen, ohne Z"), danach folgen das volle Positionierungs-Dokument und abgeleitete Bios (LinkedIn-Headline, Speaker-Bio). Zweisprachig (DE/EN). Für Firmen und Produkte ist b2b-positioning das passende Werkzeug.

**Einsatz:** *"Wofür soll ich stehen?"*, *"Schärf meine LinkedIn-Positionierung"* oder *"Stell mich in einem Satz vor."*

### proven-better-new

Validiert Produktideen mit Mark Pincus' "Proven, Better, New"-Framework (aus "Life at the Speed of Play", 2026). Erst Interview, dann Scoring gegen die Rubrik, am Ende ein klares Verdikt: BUILD, TEST FIRST, REWORK oder KILL THE IDEA, KEEP THE INSTINCT. Zweisprachig (DE/EN).

**Einsatz:** *"Validiere diese Produktidee"*, *"Sollten wir das bauen?"* oder eine Idee beschreiben und nach dem PBN-Score fragen.

### ux-audit

Führt einen strukturierten UX-Audit durch: auf Screenshots, Figma-Dateien, Live-URLs oder Recordings. Standard ist das Vollaudit mit Heuristik-Pass, Bias- und Prinzip-Linsen sowie Accessibility-Check, priorisiert nach Severity. Für den schnellen Blick gibt es den Quick-Scan.

**Einsatz:** Screenshots oder Figma-Link posten und fragen: *"Mach einen UX-Audit"* oder *"Wo verlieren wir Nutzer in diesem Flow?"* Für die kurze Variante: *"Schau kurz drüber."*

## Skills, die ich für gut befunden habe und regelmässig verwende

Neben meinen eigenen Skills nutze ich diese hier von anderen. Alle sind offen verfügbar und lohnen einen Blick.

**Design und Frontend**

- [frontend-design](https://github.com/anthropics/skills/blob/main/skills/frontend-design/SKILL.md) (Anthropic): Anleitung für UIs mit eigener visueller Identität statt generischem AI-Look, mit durchdachten Farbpaletten, Typo-Pairings und Layout-Entscheidungen.
- [taste-skill](https://github.com/Leonxlnx/taste-skill) (Leonxlnx): Sammlung für Layout, Typografie, Animation und Spacing, damit AI-Coding-Agents keine langweiligen Standard-Interfaces bauen.
- [hue](https://github.com/dominikmartn/hue) (dominikmartn): lernt eine Marke aus URL, Name oder Screenshot und macht daraus ein komplettes Design-System, das über Sessions konsistent bleibt.
- [skills for design engineers](https://github.com/emilkowalski/skills) (Emil Kowalski): Fokus auf Animation und Motion, mit Easing-Regeln, einem strengen Review-Skill und einem Vokabular, um Animationswünsche präzise zu formulieren.

**Bauen und Absichern**

- [mcp-builder](https://github.com/anthropics/skills/blob/main/skills/mcp-builder/SKILL.md) (Anthropic): Leitfaden für hochwertige MCP-Server in Python (FastMCP) oder TypeScript, wenn du externe APIs für LLMs zugänglich machst.
- [project-codeguard](https://github.com/cosai-oasis/project-codeguard) (CoSAI / OASIS): bettet sichere Coding-Praktiken direkt in die AI-gestützte Entwicklung ein, damit Agents automatisch sichereren Code schreiben.

**Marketing und Ads**

- [NotFair](https://github.com/nowork-studio/NotFair) (nowork studio): Claude-Code-Plugin mit Zugriff auf Google Ads, Meta Ads und SEO-Tools. Findet verschwendetes Budget, diagnostiziert Creative Fatigue und setzt Optimierungen direkt um.
- [adloop](https://github.com/kLOsk/adloop) (kLOsk): MCP-Server mit Lese- und Schreibzugriff auf Google Ads und GA4. Kampagnen optimieren, Conversions diagnostizieren und Tracking validieren, ohne den Dashboard-Wechsel.

## Lizenz und Nutzung

Nimm, was du brauchst, und pass es an deinen Kontext an. Die Skills sind bewusst als editierbare Markdown-Dateien gebaut: entpacken, `SKILL.md` anpassen, wieder zippen, fertig.
