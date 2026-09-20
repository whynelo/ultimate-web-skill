# Review — Auto-Review + P0/P1

**Aufgabe:** Nach dem Build fail-closed prüfen, P0/P1 selbst fixen, `REVIEW.md` schreiben.  
**Phase:** 7  
**Prompt:** `prompts/07-review.md`  
**Artefakt:** `REVIEW.md`

Jev (Typesafe) ist **optional**. Default = Agent-Review mit denselben Gates.

---

## Schwere

| Stufe | Bedeutung | Aktion |
|-------|-----------|--------|
| **P0** | Ship-Block (Legal lügt, Secrets, kein Impressum, Tracker vor Consent, Accounts ohne Alter, House-Skin-Klon, Nachmittag-leer, kein Instrument) | Sofort fixen |
| **P1** | Craft/Conversion/a11y ernst (Overflow, Dual-CTA-Kampf, Fake-proof-Risiko, Kontrast, missing sticky) | Fixen in derselben Phase |
| **P2** | Polish | Pass 4 oder Backlog, nicht als „fertig“ verstecken wenn P0/P1 offen |

---

## Scan-Achsen

Nutze Checklisten aus `redesigner-lol.md` (Anti-Slop) + `premium-passes.md` (Pass 3) + `legal-security.md` + `differentiation.md`.

1. **Lock vollständig?** Werte statt TBD  
2. **Atmosphere + Signatur-Moment + Instrument**  
3. **Nachmittag-Test** 25 % Zoom  
4. **Median-Tells** (Ghost-Wort, drei Nomen-Karten, Pink-Pille, Inter-only, Fade-up-Spam, …)  
5. **Reskin-Test** und **Sibling-Test**  
6. **Watermelon ≥3** remappt geloggt  
7. **Copy** gesprochen, keine Fake-Metriken, `lang` = Copy  
8. **Legal class** + Impressum/Datenschutz stack-treu  
9. **Mobile 390:** overflow-x 0, CTA ≥44px, kein Lenis default  
10. **Secrets / Headers / Forms**

Ab 4 strukturellen Tells: nicht „ein bisschen CSS“ — zurück zu Lock oder Ausstattung.

---

## REVIEW.md-Form

```md
# REVIEW
Datum:
Pass-Log-Stand:
## P0
- [ ] …
## P1
- [ ] …
## P2
- [ ] …
## Differentiation / Sibling
## Legal
## Watermelon slugs wired
## Verdict
ship | ship_with_lawyer_todos | hold
## Fixes applied this pass
```

Nach Fixes Datei aktualisieren. Offene P0 = kein Ship.

---

## Optional: Jev (aus redesigner-jev, adaptiert)

Nur wenn `TYPESAFE_API_KEY` gesetzt. Nie den Key committen.

`POST https://api.typesafe.ai/v1/systemone` · Model pin `jev-1.13.0` bei Kalibrierung.

Jev entscheidet **nicht** Hexes, Prosa, HTML. Jev: complete? empty? median? ship?

### Rollen

| Job | Owner |
|-----|--------|
| Fakten, Mode, Typ A–E | Human / Intake |
| Pixel, Motion, Copy | Builder |
| Lock complete? Afternoon-empty? Ship? | Jev oder Agent-Gate |

### Gate 1 — Lock

State: DESIGN-SYSTEM (kompakt). Fragen: `lock_complete` (noul) · `median_prior_risk` · `accent_fingerprint` · `house_skin_clone` · `differentiation_table` · `ausbau_locked` · `next_action`.

Act: `lock_complete < 0.7` oder `strengthen_lock` → Phase 1/2 nachziehen. House-Skin oder Fingerprint hoch → Identität ändern, nicht ein Hex.

### Gate 2 — Craft

Afternoon-empty, ein Icon-Set, eine Karten-Sprache, Fake-Proof, Choreografie.

### Gate 2b — Craft-class

Atmosphere, Signatur-Moment, Instrument, Furniture-Dichte, `matches_class_bar`, `plain_ai_template`, `watermelon_logged`. Fail → `run_premium_pass`, kein Ship.

### Gate 3 — Anti-Slop

Tell-Severity, Median vs. Empty, Reskin, Verdict (`redo_from_lock` / `ausstattung` / copy).

### Gate 4 — Ship

`legal_honest`, `legal_class_set`, `tdddg_consent_ok`, `age_gate_ok`, `secrets_safe`, `mobile_safe`, `a11y_baseline`, `ship`.

Auto-ship nur bei `ship` + Confidence ≥ 0.75 **und** Legal-Nouls ≥ 0.8 **und** secrets ≥ 0.9. Confidence < 0.5 → Mensch.

Payload ohne API-Key. Kompaktes JSON, kein Repo-Dump.

---

## Was nicht funktioniert

Jev/Agent „design a cooler hero“ fragen. Craft-class skippen. Legal-grün als Craft-grün verkaufen.
