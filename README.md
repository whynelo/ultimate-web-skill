# Ultimate Web Skill

Premium-Website-Pipeline für AI-Agenten (Cursor, Claude Code, Codex).  
**Nachfolger von `redesigner-jev`.** Skill-Körper primär Deutsch; Phasen-Namen und Frontmatter bilingual.

> DE/EU-Legal ist immer hart aktiv. One-Shot-Tailwind und House-Skin-Klone sind ein fehlgeschlagener Lauf.

---

## Deutsch

### Was das ist

Ein installierbarer Agent-Skill (`name: ultimate-web`), der eine **nicht-skipbare Pipeline** erzwingt:

0. Deep Intake → `BRIEF.md` + `INTAKE.json`  
1. Design-Intelligenz (Pro Max + Taste-Dials + frontend-design) → `DESIGN-SYSTEM.md`  
2. Godly.design-Forschung → `GODLY-DNA.md`  
3. Watermelon-Shortlist (3–7) → `WATERMELON-PLAN.md`  
4. Stitch optional (Skip dokumentieren)  
5. Mehrpass-Build (gesprochene DE-Copy, keine Fake-Metriken)  
6. Gemini-Bildprompts → `GEMINI-IMAGE-PROMPTS.md` **dem Menschen zeigen**  
7. Auto-Review → `REVIEW.md` + Auto-Fix P0/P1  
8. Endkritik (Design / Funktion / Vibe / Security) + urgente Fixes → Ship  

Immer: `modules/legal-security.md` (DSGVO, DDG, TDDDG, Alter, Security) und `modules/differentiation.md`.

### Installation

#### Cursor

**Projekt-lokal** (empfohlen für Client-Repos):

```bash
mkdir -p .cursor/skills/ultimate-web
# dieses Repo hierher klonen oder die Dateien kopieren
git clone https://github.com/whynelo/ultimate-web-skill .cursor/skills/ultimate-web
```

**Global:**

```bash
git clone https://github.com/whynelo/ultimate-web-skill ~/.cursor/skills/ultimate-web
```

Cursor lädt `SKILL.md` automatisch, wenn die Beschreibung zum Task passt. Explizit:

```
Lies ~/.cursor/skills/ultimate-web/SKILL.md und starte Phase 0.
```

#### Claude Code

```bash
mkdir -p .claude/skills
git clone https://github.com/whynelo/ultimate-web-skill .claude/skills/ultimate-web
```

Oder global nach `~/.claude/skills/ultimate-web`.

#### Codex / andere Agenten

Skill-Ordner ins projektübliche Skills-Verzeichnis kopieren (`.agents/skills/ultimate-web` oder Repo-Root). Agent muss `SKILL.md` zuerst lesen.

### Aufruf

```
Nutze den Skill ultimate-web.
Baue / redesigne <Brief oder URL>.
Pipeline 0–8, keine Phase skippen. Legal hart. Deutsch sprechen.
```

Einzelphase: `prompts/00-intake.md` … `prompts/07-review.md`.

### Erweitern

Siehe `ARCHITECTURE.md`. Kurz:

1. Neues Wissen = neues `modules/<name>.md` (eine Aufgabe).
2. Phase nur ändern, wenn der Vertrag in `SKILL.md` mitwächst (Artefakt + Prompt).
3. Upstream zitieren und paraphrasieren — keine copyrighted `SKILL.md` wholesale einfügen.
4. Keine Mega-Prompts (Lost in the Middle). Kurze Phasen-Prompts, Tokens oben anpinnen.

### Migration von redesigner-jev

Siehe `MIGRATION.md`. Dieser Skill **ersetzt** redesigner-jev vollständig.

---

## English

### What this is

A portable agent skill (`name: ultimate-web`) that **replaces redesigner-jev**. It forces a nine-phase premium website pipeline (intake → design intelligence → Godly DNA → Watermelon → optional Stitch → multi-pass build → Gemini prompts → review → final critique). **DE/EU legal is always on.**

The skill body is primarily German (author + DE clients). Phase names and the frontmatter description are bilingual so other models have a stable contract.

### Install (Cursor)

```bash
git clone https://github.com/whynelo/ultimate-web-skill ~/.cursor/skills/ultimate-web
# or project-local:
# git clone https://github.com/whynelo/ultimate-web-skill .cursor/skills/ultimate-web
```

### Install (Claude Code)

```bash
git clone https://github.com/whynelo/ultimate-web-skill .claude/skills/ultimate-web
```

### Invoke

```
Read SKILL.md from ultimate-web. Run phases 0–8 with no skips.
Brief: <facts or live URL>
```

### Extend

See `ARCHITECTURE.md`. Add modules; do not paste upstream skills wholesale; keep phase prompts short.

---

## Repo-Lage

| Pfad | Zweck |
|------|--------|
| `SKILL.md` | Vertrag, Pipeline, Hard defaults |
| `modules/` | Eine Datei = eine Aufgabe |
| `prompts/00`–`07` | Kurze Phasen-Prompts (ein Paste = ein Schritt) |
| `templates/` | Artefakt-Schablonen |
| `refs/` | Kataloge + Klassen-Hinweise |
| `ARCHITECTURE.md` | Wie man den Skill erweitert |
| `MIGRATION.md` | redesigner-jev → ultimate-web |
| `CHANGELOG.md` | Versionen |

---

## Quellen (lesen, nicht klonen)

- https://redesigner.lol/prompts · https://redesigner.lol/quellen
- https://godly.design/websites/
- https://ui.watermelon.sh/animated-components
- https://styles.refero.design/
- [ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill)
- [taste-skill](https://github.com/Leonxlnx/taste-skill) (`design-taste-frontend`)
- [Anthropic frontend-design](https://github.com/anthropics/skills/tree/main/skills/frontend-design)

Klasse (Entscheidungen stehlen, nie Hex/Logo/Copy):  
jober-a69.pages.dev · essentialz-site.pages.dev · automater.lol · redesigner.lol

---

## Disclaimer

Diese Checklisten ersetzen keine Rechtsberatung. Vor kostenpflichtigem Traffic oder sensiblen Daten: Anwalt gegenlesen lassen.

## License

MIT — siehe `LICENSE`.
