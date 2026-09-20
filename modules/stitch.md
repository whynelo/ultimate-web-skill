# Stitch — optional

**Aufgabe:** Google Stitch (oder gleichwertiges Design-to-Code) nur nutzen, wenn es in der Session wirklich da ist.  
**Phase:** 4  
**Prompt:** `prompts/04-stitch.md`

---

## Default: Skip dokumentieren

Stitch ist **kein** Pflicht-Pixel. Es ist ein optionales Zwischenartefakt zwischen DNA und Build.

Wenn eines gilt → Skip, nicht erfinden:

- Kein Stitch-Tool / keine Auth / kein MCP
- Egress blockiert stitch-Hosts
- Brief ist type-led und braucht keine Generated Screens
- Zeit: Godly + DESIGN-SYSTEM reichen

**Skip-Block** (in `DESIGN-SYSTEM.md` oder `WATERMELON-PLAN.md`):

```md
## Stitch
- available: false
- skipped_reason: <ein Satz, wahr>
- attempted_at: ISO-8601 oder "not attempted"
```

Kein Fake-Screenshot, kein „würde so aussehen“.

---

## Wenn verfügbar

1. Nur **nach** Phase 0–3. Tokens und Godly-DNA sind Input, nicht „mach mal schön“.
2. 1–3 Screens (Hero, eine Innen-Section, Mobile). Kein 12-Screen-Kit.
3. Export als Referenz, dann **neu bauen** im Projekt-Stack. Stitch-CSS nicht als Produktionsskin.
4. Taste-Dials und Differentiation gelten. House-Skin aus dem Modell verwerfen.
5. Log: was behalten (IA, Rhythmus), was verworfen (Palette, Type).

Verwandt: taste-skill `stitch-design-taste` / optionales `DESIGN.md`-Exportformat — nur als Hinweis, nicht als Abhängigkeit.

---

## Legal / Assets

Stitch-Output kann Stock-Gesichter und Generic-Copy enthalten. Nicht als echte Mitarbeiter oder Beleg shippen. DE-Copy selbst schreiben (Phase 5).
