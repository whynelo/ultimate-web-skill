# Taste — Dials / Design-Read

**Aufgabe:** Brief lesen, eine Zeile Design-Read, drei Dials setzen.  
**Phase:** 1  
**Upstream:** https://github.com/Leonxlnx/taste-skill · Skill `design-taste-frontend`  
**Vertrag (EN names, nicht umbenennen):** `DESIGN_VARIANCE` · `MOTION_INTENSITY` · `VISUAL_DENSITY`

Paraphrase, kein Wholesale-Dump des Upstream-SKILL.

---

## Design-Read zuerst

Signale: Page-Kind · Vibe-Wörter · Referenz-URLs · Audience · vorhandene Brand-Assets · stille Constraints (a11y, reguliert, Kids).

Eine Zeile, dann Dials. Bei echter Divergenz **eine** Klärfrage — keine Frage-Lawine.

Anti-Default: AI-Lila-Mesh, zentrierter Dark-Hero, drei Feature-Cards, Glass überall, Inter+slate-900 als Autopilot.

---

## Die drei Dials (1–10)

| Dial | 1 | 10 | Baseline |
|------|---|----|----------|
| `DESIGN_VARIANCE` | Symmetrie, ruhig | Asymmetrie, artig | 8 |
| `MOTION_INTENSITY` | Fast still | Cinematic / Physik | 6 |
| `VISUAL_DENSITY` | Galerie / Luft | Cockpit | 4 |

Baseline `8 / 6 / 4` nur wenn der Read Marketing/Portfolio ohne Extra-Signal ist. **Nicht** den User die Datei editieren lassen — conversational überschreiben.

### Inferenz (Richtwerte)

| Signal | VAR | MOT | DEN |
|--------|-----|-----|-----|
| minimal / calm / editorial / Linear | 5–6 | 3–4 | 2–3 |
| premium / Apple-adjacent / luxury | 7–8 | 5–7 | 3–4 |
| Awwwards / experimental / Agency | 9–10 | 8–10 | 3–4 |
| Marketing default | 7–9 | 6–8 | 3–5 |
| trust-first / public / regulated | 3–4 | 2–3 | 4–5 |
| Redesign preserve | match | match+1 | match |
| Redesign overhaul | +2 | +2 | match |
| Handwerk / lokale Broschüre | 5–7 | 3–5 | 4–6 |
| SaaS tool-dock | 6–7 | 5–6 | 4–5 |

Handwerk darf **dichter** sein als Agency-Luft (Ausstattung), ohne VARIANCE 10.

---

## Wie Dials die Seite treiben

- **VARIANCE niedrig:** Satzspiegel, eine Spalte, wenig Breakouts. Hoch: 7fr/5fr, overlap, ein Ausbruch.
- **MOTION niedrig:** Struktur trägt (Gitter, Zahlen, Rahmen). Hoch: ein Hero-Wow + Choreografie — nicht Fade-up-Spam. Redesigner-Budget bleibt: 1 Wow + 1 Ambient.
- **DENSITY niedrig:** still / wenige Blöcke. Hoch: ausgestattet/voll — echte Inhalte, nicht Dummy-Karten.

Dials widersprechen nicht `modules/premium-passes.md`: MOTION 9 ist kein Freifahrtschein für Lenis auf iPhone.

---

## Design-System-Ehrlichkeit

Wenn der Brief nach einem **offiziellen** System klingt (GOV.UK, USWDS, Polaris, Fluent, Carbon, Primer): das Paket nutzen, nicht nachbauen. **Ein** System pro Projekt.

Wenn der Brief eine **Ästhetik** ist (Editorial, Brutal, Glass, Kinetic): native CSS / Tailwind + ehrlich kommentieren. „Apple Liquid Glass“ im Web = Approximation (`backdrop-filter`), so labeln.

---

## Output in DESIGN-SYSTEM.md

```
## Taste
- design_read: "Reading this as: …"
- DESIGN_VARIANCE: n
- MOTION_INTENSITY: n
- VISUAL_DENSITY: n
- override_reason: (wenn nicht Baseline)
```
