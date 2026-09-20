# Watermelon — Motion-Rezepte / Animated recipes

**Aufgabe:** 3–7 Rezepte shortlisten, auf Godly-DNA remappen, später installieren.  
**Phase:** 3 (Plan) + Phase 5 Pass 2 (Install)  
**Quellen:** https://ui.watermelon.sh/animated-components · `refs/watermelon-animated.json` (131 Slugs)  
**Artefakt:** `WATERMELON-PLAN.md`  
**Prompt:** `prompts/03-watermelon.md`

Inventar adaptiert aus redesigner-jev `WATERMELON-ANIMATED.md` — Katalog bleibt JSON, dieses Modul ist der **Vertrag**.

---

## Hart

- Marketing-Site: Shortlist **3–7**, davon ≥3 wirklich verdrahtet (oder Custom-Signature mit Motion-Values).
- Install: `npx shadcn@latest add https://registry.watermelon.sh/r/<slug>.json` **oder** Rezept portieren (Astro Islands).
- **Alle Tokens remappen.** Nie Watermelon-Demo Lime/Pink/Inter.
- Hero braucht ein Instrument (Watermelon oder Custom). Headline+Buttons allein = Fail.
- `prefers-reduced-motion`: Endzustand sofort.
- Slugs in README / Pass-Log / `WATERMELON-PLAN.md`.

---

## Auswahl nach Site-Typ

| Typ | Bevorzugen | Nicht als Default |
|-----|------------|-------------------|
| Handwerk / lokal | `slot-picker`, `schedule-button`, `calendar-widget`, `onboarding-checklist`, `card-split-accordian`, `floating-input`, `expandable-profile-card`, `shimmer-button`, `view-on-map` (privacy-safe / Facade) | Crypto-Swap, Emoji-Spree |
| SaaS / Tool | `onboarding-checklist`, `morphing-button`, `credit-usage-card`, `carousel-navigator`, `dock`, `command-search` | Random Finance-Widgets |
| Shop / Streetwear | `card-swipe`, `carousel-slider`, `radial-carousel`, `shimmer-button` | Onboarding-Setup-Spam |
| Portfolio / Agency | `carousel-navigator`, `expandable-event-card`, `activities-card`, `revealing-cards` | Budget/Trade-Cards |

Godly-DNA gewinnt: ein stilles Editorial bekommt kein Radial-Carousel nur weil es „wow“ ist.

---

## Plan-Tabelle (Pflicht)

| Role | Slug | Why (1 Satz) | Page | Godly-remap (Token/Timing) |
|------|------|--------------|------|----------------------------|

Rollen-Beispiele: `hero-instrument` · `primary-cta` · `faq` · `booking` · `proof-gallery` · `team` · `micro`.

---

## Install-Notizen (Phase 5)

- Astro: `client:visible` / `client:load` nur auf interaktiven Islands.
- Eine Motion-Lib (`motion/react`) — nicht Framer + GSAP + Lenis stapeln.
- Dependencies des Slugs prüfen; unused Icon-Packs nicht als zweites Icon-Set einschleppen (ein Set bleibt Gesetz).
- Demo-Copy und Demo-Zahlen streichen.
- Mobile: Gesten dürfen natives Scroll nicht stehlen.

---

## Katalog

131 Unique Slugs, 26 Kategorien — siehe `refs/watermelon-animated.json` und `refs/README.md`.  
Nicht den ganzen Katalog in den Chat dumpen. Shortlist begründen.
