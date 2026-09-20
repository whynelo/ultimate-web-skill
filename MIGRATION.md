# Migration: redesigner-jev → ultimate-web

**DE:** Dieser Skill **ersetzt** redesigner-jev vollständig.  
**EN:** This skill is the successor. Do not run both stacks on one site.

---

## Warum / Why

redesigner-jev war: Redesigner-Lauf + Refero + Watermelon + Jev-Gates + DE-Legal.  
Das war richtig — und unvollständig. Es fehlten:

- hartes **Intake** (BRIEF + INTAKE.json) vor dem Lock
- **Design-Intelligenz** als eigene Phase (Pro Max + Taste-Dials + frontend-design)
- **Godly.design** als Pflicht-DNA, nicht nur Link in /quellen
- **Gemini-Prompts** als sichtbares Artefakt
- **Auto-Review + Endkritik** unabhängig von Jev-API
- ein Repo, das Agenten als `name: ultimate-web` laden

Jev bleibt **optional** (Gate-Packs in `modules/review.md`), ist aber nicht mehr der Namensgeber.

---

## Mapping

| redesigner-jev | ultimate-web |
|----------------|--------------|
| `SKILL.md` (Redesigner + Jev) | `SKILL.md` (`ultimate-web`) + Pipeline 0–8 |
| Redesigner 01 Lock | Phase 1 `DESIGN-SYSTEM.md` **nach** Phase 0; Lock-Felder bleiben |
| 02 Viewport … 07 Legal | **innerhalb** Phase 5 (Build), Tokens aus 0–3 |
| `LEGAL-SECURITY.md` | `modules/legal-security.md` (immer, hart) |
| `DIFFERENTIATION.md` | `modules/differentiation.md` (immer) |
| `PREMIUM-PASSES.md` | `modules/premium-passes.md` (Phase 5) |
| `QUALITY-BAR.md` | verteilt: `premium-passes` + `review` + `redesigner-lol` |
| `JEV-REVIEW.md` / `JEV-COLLAB.md` | `modules/review.md` (Auto-Review default; Jev wenn Key) |
| `WATERMELON-ANIMATED.md` + JSON | `modules/watermelon.md` + `refs/watermelon-animated.json` |
| `REFERO-STYLES.md` | `modules/refero.md` (Phase 1/2, nicht statt Godly) |
| WhyNelo SHARED-CORE / VERSION-2 | `modules/redesigner-lol.md` + `modules/intake.md` (Mode 2) |
| — | Phase 2 Godly, Phase 4 Stitch, Phase 6 Gemini, Phase 8 Critique |

---

## Install-Pfad ändern

| Alt | Neu |
|-----|-----|
| `.cursor/skills/redesigner-jev/` | `.cursor/skills/ultimate-web/` |
| `.claude/skills/redesigner-jev/` | `.claude/skills/ultimate-web/` |

Altes Verzeichnis löschen oder umbenennen, damit Agenten nicht zwei widersprüchliche Skills laden.

```bash
rm -rf ~/.cursor/skills/redesigner-jev ~/.claude/skills/redesigner-jev
git clone https://github.com/whynelo/ultimate-web-skill ~/.cursor/skills/ultimate-web
```

---

## Laufende Projekte

1. Existierende `DESIGN.md` behalten. Phase 0–3 **nachziehen**: `BRIEF.md`, `INTAKE.json`, `DESIGN-SYSTEM.md` (kann auf DESIGN.md verweisen), `GODLY-DNA.md`, `WATERMELON-PLAN.md`.
2. House-Skin-Check (`modules/differentiation.md`) — wenn void+Acid+Magenta ohne Auftrag: Lock neu.
3. Pass-Log auf ≥ Pass 3 prüfen; sonst Phase 5 weiterlaufen.
4. `REVIEW.md` + Endkritik einmalig nachziehen, auch wenn die Site schon live ist.
5. Jev-Calls: gleiche Packs, neuer Ort (`modules/review.md`). Pin weiter `jev-1.13.0` wenn kalibriert.

---

## Was sich für den Menschen ändert

- Agent fragt zuerst (Phase 0), statt sofort DESIGN.md zu schreiben.
- Godly-URLs und Watermelon-Slugs sind Pflicht-Artefakte, keine „nice to have“.
- Gemini-Prompts erscheinen im Chat, nicht nur als stille Datei.
- „Legal OK“ allein reicht nicht mehr — Craft-class + Differentiation + Critique.

---

## Was sich nicht ändert

- DE/EU-Checkliste, Alter 16/18, keine erfundenen Registerdaten
- Spoken DE, ein Icon-Set, eine Karten-Sprache
- Watermelon remap, nie Demo-Skin
- Klasse jober / essentialz / automater / redesigner.lol = Entscheidungen, nicht Hexes
- Fail-closed auf Nachmittag-leer und Agency-Median
