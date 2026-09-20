# Final Critique — Endkritik / Ship

**Aufgabe:** Nach Review vier Achsen hart bewerten, Urgentes fixen, dann erst Ship.  
**Phase:** 8  
Kein eigener `0N`-Prompt — unmittelbar nach Phase 7, ohne Skip.

---

## Vier Achsen / Four axes

### 1. Design

- First Viewport ≤3s: Canvas → Atmosphere → Vignette → Typ (optisches Drittel) → eine Handlung → Instrument/Moment
- Type-Scale und Rhythmus aus DESIGN-SYSTEM, nicht Tailwind-Defaults
- Godly-DNA erkennbar als *Entscheidung*, nicht als Clone
- Differentiation + Sibling ≤2s ohne Wordmark

### 2. Funktion

- Primär-CTA durchgängig (Hero, Mid, Sticky, Footer)
- Forms: Labels, Fehler, Rate-Limit/Honeypot, Zweck + Datenschutz-Link
- Mode 2: Conversion-Pfade der Live-Site existieren noch
- Build grün; tote Links; `tel:` / Mail stimmen mit NAP
- Keine Hover-only-kritische Info

### 3. Vibe

- Spoken Copy, keine AI-Kicker („unlock the future“, Gedankenstrich-Regen, Title-Case-Buttons)
- Eine Primitive, eine Material-Sprache
- Nicht nachmittag-leer, nicht Agency-Median
- Reduced-motion: lesbar im Stillstand
- Team/Über-uns teilt die Markenwelt der Home (Tint ok, kein zweites Theme)

### 4. Security + Legal

- `modules/legal-security.md` Ship-Blocker
- Secrets nicht im Client
- Stack-treues Datenschutz
- Alter serverseitig bei C/D
- Dependency-Audit bei C+ sinnvoll

---

## Urgent vs. later

**Urgent (fix now):** alles P0, plus Vibe-Brüche die den Reskin-/Sibling-Test knacken, plus Conversion-Sackgassen.

**Later:** P2-Typo-Feinschliff, zweites Micro, optionales Pass E wenn User nicht „plain“ gesagt hat.

---

## Ship-Gate

Ship nur wenn:

- REVIEW Verdict `ship` oder `ship_with_lawyer_todos` (TODOs in README)
- Phase-6-Prompts dem User gezeigt
- Pass-Log ≥ 3
- Legal class + Impressum/Datenschutz
- Watermelon-Log
- Differentiation-Tabelle gefüllt

Sonst: zurück zur genannten Phase, nicht „ein letztes CSS“.

---

## Handoff

README (DE bei DE-Kunden): Install, wo NAP liegt, Motion-Log, Processors/AVV, Lawyer-Disclaimer, Refero/Godly/Watermelon-Credits (inspiriert, keine Endorsements).
