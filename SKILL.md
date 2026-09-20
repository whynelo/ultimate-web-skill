---
name: ultimate-web
description: >-
  DE: Vollständige Premium-Website-Pipeline für Cursor, Claude Code und Codex.
  Nutze diesen Skill, wenn eine Site gebaut, redesigned oder von Null aufgezogen
  wird — Intake → Design-Intelligenz → Godly-DNA → Watermelon → optional Stitch
  → Mehrpass-Build → Gemini-Bildprompts → Auto-Review → Endkritik.
  DE/EU-Legal (DSGVO, DDG, TDDDG) ist immer hart aktiv. Nicht für One-Shot-Tailwind,
  House-Skin-Klone oder Versand ohne Pass 3 / Review.
  EN: Complete premium website pipeline for Cursor, Claude Code, and Codex.
  Use when building, redesigning, or greenfielding a site — intake → design
  intelligence → Godly DNA → Watermelon → optional Stitch → multi-pass build →
  Gemini image prompts → auto-review → final critique. DE/EU legal is a hard
  always-on module. Do not use for one-shot Tailwind, house-skin clones, or
  shipping without Pass 3 / review.
---

# Ultimate Web

**Nachfolger von redesigner-jev.** Eine harte, nicht-skipbare Pipeline für Premium-Sites in der Klasse von jober / essentialz / automater / redesigner.lol — plus Design-Intelligenz (Pro Max, Taste-Dials, frontend-design), Godly-DNA und Watermelon-Motion.

Skill-Körper primär **Deutsch** (Klaas + DE-Kunden). **Englische Phasen-Namen** und Dual-Headings sind der Vertrag für andere AIs. **DE/EU Legal = hartes Modul, immer.**

> Flat / AI-plain / House-Skin-Klon = fehlgeschlagener Lauf. Legal-grün ≠ Craft-grün.

---

## Wann nutzen / When to use

| Nutzen | Nicht nutzen |
|--------|----------------|
| Neue Site, Redesign, Portfolio, Handwerk, SaaS-Marketing, Agency | Reines Backend, Infra, One-Shot-„mach mal Tailwind“ |
| User sagt „premium“, „geil“, „nicht KI“, „wie redesigner“ | House-Skin (void + Acid-Lime + Magenta) ohne Marken-Auftrag |
| DE/EU-facing mit Impressum/Datenschutz | Versand ohne Intake, Godly-DNA oder Review |

**Invoke (Cursor / Claude / Codex):**

```
Lies SKILL.md von ultimate-web und führe die Pipeline 0–8 ohne Skip aus.
Brief: <URL oder Fakten>
```

Oder Phasen einzeln: `prompts/00-intake.md` … `prompts/07-review.md`, danach Modul `final-critique`.

---

## Hard rule — keine Phase überspringen

Der Agent **darf keine Phase auslassen**. Phase 4 (Stitch) ist die einzige optionale; Skip muss in `WATERMELON-PLAN.md` oder `DESIGN-SYSTEM.md` **dokumentiert** werden (warum unavailable).

| # | Phase (EN contract) | DE | Pflicht-Artefakt | Modul |
|---|---------------------|----|------------------|--------|
| 0 | Deep Intake Q&A | Tiefen-Briefing | `BRIEF.md` + `INTAKE.json` | `modules/intake.md` |
| 1 | Design Intelligence | Design-Intelligenz | `DESIGN-SYSTEM.md` | `ui-ux-pro-max` + `taste` + `frontend-design` |
| 2 | Godly DNA | Godly-Forschung | `GODLY-DNA.md` | `modules/godly.md` |
| 3 | Watermelon Plan | Motion-Shortlist | `WATERMELON-PLAN.md` | `modules/watermelon.md` |
| 4 | Stitch | Optional | Skip-Notiz oder Stitch-Export | `modules/stitch.md` |
| 5 | Build | Premium-Mehrpass | Site + Pass-Log | `premium-passes` + `redesigner-lol` |
| 6 | Gemini Image Prompts | Bildprompts | `GEMINI-IMAGE-PROMPTS.md` **dem User zeigen** | `modules/gemini-images.md` |
| 7 | Auto Review | Auto-Review + Fix | `REVIEW.md` + P0/P1 gefixt | `modules/review.md` |
| 8 | Final Critique | Endkritik + Ship | Critique + urgente Fixes | `modules/final-critique.md` |

**Immer geladen (kein Skip):** `modules/legal-security.md` · `modules/differentiation.md`

Templates: `templates/`.

---

## Lesereihenfolge / Read first

1. Dieses File (Vertrag + Pipeline)
2. `modules/legal-security.md` — DE/EU Pflicht
3. `modules/differentiation.md` — Site ≠ letzte Site
4. Phase-Modul + passender Prompt
5. `modules/redesigner-lol.md` — Redesigner-Prompts, Quellen, WhyNelo SHARED-CORE / VERSION-2
6. `modules/premium-passes.md` — Mehrpass, Anti-Plain
7. `ARCHITECTURE.md` — erweitern, nicht aufblasen

Upstream (paraphrasieren, **nicht** wholesale dumpen):

- https://redesigner.lol/prompts · https://redesigner.lol/quellen
- https://godly.design/websites/
- https://ui.watermelon.sh/animated-components
- https://styles.refero.design/
- https://github.com/nextlevelbuilder/ui-ux-pro-max-skill
- https://github.com/Leonxlnx/taste-skill (`design-taste-frontend`)
- Anthropic frontend-design: https://github.com/anthropics/skills/tree/main/skills/frontend-design

---

## Pipeline (hart)

### Phase 0 — Deep Intake / Tiefen-Briefing

Stelle gezielte Fragen (nicht 40 auf einmal). Fülle `BRIEF.md` + `INTAKE.json`.

Pflicht: Mode 1/2/3 · Typ A–E · Legal class A–E · Anrede Du/Sie · echte Angebote · NAP oder ehrliche Platzhalter · Assets-Provenienz · Conversion-Handlung · Cut-Liste.

**Nie erfinden:** HRB, USt, Reviews, „seit 2014“, Partnerlogos, Fake-Metriken.

→ `modules/intake.md` · `prompts/00-intake.md`

### Phase 1 — Design Intelligence / Design-Intelligenz

Bevor Pixel: Pro-Max-Reasoning (Produkt→Pattern→Style→Anti-Pattern) + Taste-Dials (`DESIGN_VARIANCE` / `MOTION_INTENSITY` / `VISUAL_DENSITY`) + frontend-design (Purpose → Aesthetic → Type/Color/Composition/Interaction).

Output: `DESIGN-SYSTEM.md` mit Tokens, Komposition, Signatur-Moment, Differentiation-Tabelle, Legal class, Ausbau-Stufe.

→ `modules/ui-ux-pro-max.md` · `modules/taste.md` · `modules/frontend-design.md` · `prompts/01-design-intelligence.md`

### Phase 2 — Godly DNA

Öffne https://godly.design/websites/, wähle 1–3 URLs die **zu diesem Brief** passen (nicht die trendigste Karte). Extrahiere: Type-Scale, Spacing, Rhythmus, Motion, Hierarchie, Material. Remap auf **diese** Marke.

Output: `GODLY-DNA.md`

→ `modules/godly.md` · `prompts/02-godly.md` · ergänzend `modules/refero.md`

### Phase 3 — Watermelon Plan

https://ui.watermelon.sh/animated-components + `refs/watermelon-animated.json` (131 Rezepte). Shortlist **3–7** Slugs, Rollen-Mapping, Remap auf Godly-DNA. Nie Demo-Skin (Lime/Pink/Inter).

Output: `WATERMELON-PLAN.md`

→ `modules/watermelon.md` · `prompts/03-watermelon.md`

### Phase 4 — Stitch (optional)

Google Stitch nur wenn Session/Tool verfügbar. Sonst: `skipped: true` + Grund. Nicht erfinden, nicht hinter Login scrapen.

→ `modules/stitch.md` · `prompts/04-stitch.md`

### Phase 5 — Build / Premium-Mehrpass

Mehrpass laut `modules/premium-passes.md`. Spoken DE-Copy wenn Brief DE. Keine AI-Kicker, keine Fake-Metriken. Hero braucht ein echtes Instrument. Pass-Log ≥ Pass 3 vor „fertig“.

Redesigner-Schritte 01–07 (Lock → Viewport → Rest → Ausstattung → Texte → Anti-Slop → Legal) sitzen **innerhalb** dieser Phase, nachdem 0–4 Artefakte existieren.

→ `modules/premium-passes.md` · `modules/redesigner-lol.md` · `prompts/05-build.md`

### Phase 6 — Gemini Image Prompts

Schreibe `GEMINI-IMAGE-PROMPTS.md` (Hero, Material, Team-Platten nur als Platzhalter-Art, nie Fake-Mitarbeiter). **Datei dem User zeigen** — nicht still ins Repo legen.

→ `modules/gemini-images.md` · `prompts/06-gemini-images.md`

### Phase 7 — Auto Review

`REVIEW.md`: Craft, Anti-Slop, Differentiation, Legal/Security, a11y, Mobile. **P0/P1 automatisch fixen**, dann Review aktualisieren.

→ `modules/review.md` · `prompts/07-review.md`

### Phase 8 — Final Critique

Vier Achsen: Design · Funktion · Vibe · Security. Urgente Findings fixen, dann Ship-Gate.

→ `modules/final-critique.md`

---

## Layer-Stack

| Layer | Rolle |
|-------|--------|
| Intake | Fakten, Mode, Legal class — nichts erfinden |
| Pro Max + Taste + frontend-design | Intelligenz vor Pixeln |
| Godly + Refero | echte Systeme studieren, Tokens remappen |
| Watermelon | Motion-Rezepte nach Lock |
| Redesigner 01–07 | Komposition, Viewport, Ausstattung, gesprochene Copy |
| Premium-Passes | ≥3 Pässe, Conversion, Anti-Plain |
| Legal-Security | DE/EU hart, immer |
| Differentiation | ≥3 Achsen vs. letzte Skill-Site |
| Review + Critique | fail-closed, dann Ship |

---

## Hard defaults (nicht verhandelbar)

- **SHARED-CORE + VERSION-2** (WhyNelo): Apple-artige Hierarchie, Typ, Raum; Wow max. eins; Netlify-easy für Typ A. Siehe `modules/redesigner-lol.md`.
- **Legal class A–E** in `DESIGN-SYSTEM.md` + Checkliste `modules/legal-security.md` vor Ship.
- **Differentiation Lock** — nie das House-Package (void `#07070A` + Acid `#C8FF3D` + Magenta `#FF2BD6` + Glass-Rim + Dual-Orbs + Unbounded/Outfit + Rack-Hero), außer DIESE Marke besitzt die Linie.
- Jede neue Site ändert **≥3 Achsen** gegenüber der letzten Skill-Site des Users.
- Spoken DE wenn Brief DE. Buttons: Verb + Nomen. Kein „Mehr erfahren“ als Primär-CTA.
- Self-hosted Fonts (woff2). Kein stilles Google-Fonts-CDN.
- Hero: Atmosphere + benannter Signatur-Moment + Instrument (oder bewusste type-led Stille). Headline+zwei Buttons auf Flat = Fail.
- Marketing-Site: ≥3 Watermelon-derived Interactions, Tokens remappt.
- Kein Mascot außer User fragt; ein Icon-Set; eine Karten-Sprache.
- Fail-closed auf plain / boring / AI-Template, auch wenn Routen existieren.

---

## Done when / Fertig wenn

- Artefakte 0–3 und 6–8 existieren; Phase 4 dokumentiert
- Pass-Log ≥ Pass 3 · Craft-class erfüllt · Watermelon geloggt
- Differentiation + Sibling-Test OK
- Legal OK · Secrets safe · Build grün
- Conversion-Pfad klar · **nicht plain**
- `GEMINI-IMAGE-PROMPTS.md` dem User gezeigt

---

## Secrets

`TYPESAFE_API_KEY` nur in Env (optional, Jev-Gates in `modules/review.md`). Nie committen. Gemini/OpenAI-Keys nur Server.
