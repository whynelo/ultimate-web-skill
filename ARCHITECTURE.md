# Architecture — Ultimate Web Skill erweitern

**DE:** Wie dieser Skill wächst, ohne wieder ein 45-kB-Mega-Paste zu werden.  
**EN:** How to extend the skill without recreating Lost-in-the-Middle mega-prompts.

---

## Prinzip / Principle

Sieben kurze Texte schlagen ein Ultimate-Kleister. Modelle lesen Anfang und Ende; die Mitte stirbt ([Liu et al. 2023](https://arxiv.org/abs/2307.03172)). Deshalb:

| Darf wachsen | Darf nicht wachsen |
|--------------|-------------------|
| Neue `modules/*.md` mit **einer** Aufgabe | `SKILL.md` als Dump aller Regeln |
| Ein Phasen-Prompt bleibt ein Paste | Zwei Pipelines parallel (alte 01–07 **und** 0–8 unverbunden) |
| Kataloge in `refs/` (JSON, Listen) | Copyrighted Upstream-`SKILL.md` wholesale |
| Template-Felder | Neue Default-Ästhetik (House-Skin) |

`SKILL.md` = Vertrag + Lesereihenfolge + Hard defaults.  
Module = Tiefe.  
Prompts = der Lauf.

---

## Dateivertrag / File contract

```
SKILL.md                 # name: ultimate-web · Pipeline 0–8 · wann nutzen
modules/<task>.md        # eine Aufgabe, DE-Körper, EN-Überschriften für Verträge
prompts/0N-<phase>.md    # ein Schritt, endet mit STOP, pinnt Tokens
templates/<ARTEFAKT>     # leere Pflichtfelder, keine Beispiel-Hexes der House-Linie
refs/                    # Kataloge + README, keine Pixel-Klone
```

Neue Phase nur wenn **alle** gelten:

1. Englischer Phasen-Name (Contract) + deutscher Name
2. Pflicht-Artefakt mit Template
3. Prompt in `prompts/`
4. Zeile in der Pipeline-Tabelle in `SKILL.md`
5. Eintrag in `CHANGELOG.md`

Phase 4 (Stitch) bleibt die einzige dokumentiert-skippbare.

---

## Module hinzufügen

1. Datei `modules/<kebab-name>.md` anlegen.
2. Kopf: Aufgabe in einem Satz, wann laden, welches Artefakt.
3. Regeln paraphrasieren; Upstream-URL zitieren.
4. In `SKILL.md` Lesereihenfolge oder Phase verlinken — nicht den Inhalt kopieren.
5. Falls Agent-Verhalten sich ändert: Prompt der betroffenen Phase anpassen.

### Bestehende Module (nicht umbenennen ohne Migration)

| Modul | Aufgabe |
|-------|---------|
| `intake` | Fragen, BRIEF, INTAKE.json, Modes 1–3 |
| `ui-ux-pro-max` | Produkt→Pattern→Style→Anti-Pattern (Pro Max, paraphrasiert) |
| `taste` | DESIGN_VARIANCE / MOTION_INTENSITY / VISUAL_DENSITY |
| `frontend-design` | Purpose → Aesthetic → Type/Color/Composition/Interaction |
| `godly` | godly.design lesen, DNA extrahieren |
| `watermelon` | Shortlist 3–7, Remap, Install |
| `stitch` | Optional + Skip-Protokoll |
| `gemini-images` | Prompts schreiben und **zeigen** |
| `review` | REVIEW.md + P0/P1 + optionales Jev |
| `final-critique` | Design/Funktion/Vibe/Security |
| `legal-security` | DE/EU hart, immer |
| `differentiation` | Anti-House-Clone |
| `premium-passes` | Mehrpass-Leiter, Pass E |
| `redesigner-lol` | Prompts, Quellen, SHARED-CORE / VERSION-2 |
| `refero` | styles.refero.design als Lock-Forschung |

---

## Was aus Upstream darf

| Quelle | Erlaubt | Verboten |
|--------|---------|----------|
| redesigner.lol/prompts · /quellen | Regeln paraphrasieren, URLs listen | Ganze Prompt-Bibliothek 1:1 als „Ultimate“ kleben |
| WhyNelo SHARED-CORE / VERSION-2 | Prinzipien (Klarheit, Hierarchie, Netlify-easy, Audit-first) | Fremde Client-Daten, bezahlte Packs |
| ui-ux-pro-max-skill | Prioritäten, Reasoning-Idee, Checklisten-Struktur | Dataset/CSV oder SKILL wholesale |
| taste-skill | Dials + Design-Read + Anti-Default | Vollen SKILL-Text |
| Anthropic frontend-design | Prozess purpose→aesthetic→… | Copyrighted SKILL 1:1 |
| Watermelon / Godly / Refero | Öffentliche Katalog-Metadaten, beobachtete Struktur | Paid Content rekonstruieren, Demo-Skin shippen |

---

## Artefakte im Zielprojekt (nicht in diesem Repo)

Der Skill schreibt ins **Client-Repo**:

```
BRIEF.md
INTAKE.json
DESIGN-SYSTEM.md
GODLY-DNA.md
WATERMELON-PLAN.md
GEMINI-IMAGE-PROMPTS.md
REVIEW.md
```

Plus optionale `FINAL-CRITIQUE.md`. Pass-Log und Legal class leben in `DESIGN-SYSTEM.md` (oder `DESIGN.md` wenn das Projekt den Redesigner-Namen behält — dann Querverweis).

---

## Agent-Verhalten beim Erweitern

- Eine Nachricht = ein Schritt (Cursor). v0/Lovable: 0+1 oft zusammen, Rest extra.
- Tokens oben anpinnen (Komposition, Moment, Dials, Godly-URLs, Watermelon-Slugs).
- Neue Verbote sind teuer: lange Ban-Listen aktivieren oft das Verbotene. Lieber **positive Werte** locken.
- Tests für den Skill selbst: Dateibaum vollständig, Frontmatter gültig, Pipeline-Tabelle ↔ Prompts 00–07 ↔ Module.

---

## Versionierung

Semver in `CHANGELOG.md`.

- **Patch:** Tippfehler, klarere DE-Formulierung, Katalog-Update
- **Minor:** neues optionales Modul, neues Template-Feld
- **Major:** Phase entfernt/ersetzt, Artefakt-Namen brechen, Migration nötig
