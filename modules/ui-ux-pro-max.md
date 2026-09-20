# UI/UX Pro Max — Design-Intelligenz (paraphrasiert)

**Aufgabe:** Produkt → Pattern → Style → Farbe/Typo → Anti-Pattern, **bevor** Code.  
**Phase:** 1  
**Upstream:** https://github.com/nextlevelbuilder/ui-ux-pro-max-skill — **paraphrasieren, nicht wholesale kopieren.**  
Optional lokal: `uipro init` / Search-CLI des Upstream-Repos, wenn installiert.

---

## Wann / When

Phase 1, zusammen mit `taste.md` und `frontend-design.md`.  
Skip nur bei reinem Backend — hier nie.

---

## Reasoning (Idee, nicht Dataset)

1. **Produkttyp** benennen (Handwerk, Praxis, SaaS, Portfolio, Shop, Fintech, …).
2. **Landing-Pattern** wählen (Hero-centric + Trust, Split-Offer, Editorial chapter, Product-dock, Foto-Leiter, …) — zur Conversion, nicht zur Galerie.
3. **Style** an Produkt binden (ein System). Kein Flat+Skeuo-Mix.
4. **Farbe/Typo-Mood** aus Branche + Brief, dann **eigene Hexes** (Fingerprint-Bans in `differentiation.md`).
5. **Anti-Patterns der Branche** explizit: z. B. Banking ≠ Neon-Mesh; Kanzlei ≠ Clay-Mascot; Health ≠ Heilversprechen.
6. **Pre-Delivery-Checks** in `DESIGN-SYSTEM.md` übernehmen (Kontrast, Fokus, Touch 44px, reduced-motion, 390px).

Wenn der Upstream-CLI im Projekt liegt: `--design-system` nutzen und das Ergebnis **remappen** (Fonts self-host, keine Google-CDN-Defaults, keine Montserrat-als- Luxus-Autopilot).

---

## Prioritäten (destilliert)

Reihenfolge, wenn etwas knappt — nicht alle 99 Guidelines dumpen:

| Prio | Kategorie | Muss | Anti |
|------|-----------|------|------|
| 1 | Accessibility | 4.5:1, Fokus, Labels, `h1→`, reduced-motion | Fokus-Ringe löschen, Icon-only ohne Name |
| 2 | Touch | ≥44px, 8px Abstand, Press-Feedback | Hover-only Bedeutung |
| 3 | Performance | AVIF/WebP, CLS, Fonts lokal | Layout-Thrash, 4K-Autoplay |
| 4 | Style | Ein System, ein Icon-Set (SVG) | Emoji-als-Icon, Stil-Mix |
| 5 | Layout | Mobile-first, kein Overflow-x | `100vw`+Padding, Zoom verbieten |
| 6 | Type/Color | Body ≥16px, semantische Tokens | Gray-on-gray, Raw-Hex im Component |
| 7 | Motion | 150–300ms Micro, Bedeutung | Width/Height-Animate, kein RM |
| 8 | Forms | Label am Feld, Fehler am Feld | Placeholder-only Label |
| 9 | Nav | Eine primäre Handlung, vorhersehbar | Überladene Mega-Nav ohne IA |
| 10 | Charts | Legende + nicht nur Farbe | Farbe als einzige Encoding |

---

## Branchen-Hinweise (kurz, selbst ableiten)

- **Handwerk / lokal:** Foto der Arbeit oder type-led. Leistungen als Definitionsliste. Sticky Tel. Keine drei Nomen-Karten.
- **Praxis / Health:** HWG — keine Heil-Garantie. Vertrauen vor Wow. Foto-Rechte.
- **SaaS:** Instrument im Hero (UI-Chrome echt oder ehrlicher Mock). Ein CTA.
- **Portfolio / Agency:** Dichte Ausstattung, eigene Primitive, Sibling-Test.
- **Shop:** Preise inkl. Steuer klar, Widerruf in der IA (Legal D).
- **Fintech:** Kein Spielzeug-Clay, kein Fake-Yield.

---

## Output in DESIGN-SYSTEM.md

```
## Pro Max
- product_type:
- landing_pattern:
- style_family:
- color_mood: (warum, nicht nur Hex)
- typography_mood:
- effects: ( sparsam )
- anti_patterns: (Branche + AI-Tells)
```

Fonts aus Paarungs-Empfehlungen **self-hosten**. Pro-Max-Default „Google Fonts link“ hier **überschreiben**.
