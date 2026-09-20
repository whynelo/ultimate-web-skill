# Premium-Passes — Mehrpass-Craft (Pflicht)

**Aufgabe:** Premium entsteht nicht im One-Shot. ≥3 Agent-Pässe, explizites Watermelon + Conversion.  
**Phase:** 5  
Adaptiert aus redesigner-jev `PREMIUM-PASSES.md` + Quality-Bar.

Flat/plain/boring = **failed Craft-class**. Legal-grün ≠ craft-grün.

---

## Pass-Leiter (nicht skippen)

Log in `DESIGN-SYSTEM.md` → `## Pass log` (Datum, Delta, Watermelon-Slugs).

### Pass 0 — Lock (vor Pixeln)

Bereits durch Phase 0–3 vorbereitet. Vor dem ersten Viewport prüfen:

- Godly-URLs + Remap
- Refero 1–2 **oder** Begründung
- Differentiation-Tabelle
- Legal class
- Signatur-Moment + Atmosphere
- Watermelon-Shortlist 3–7
- Conversion-Map: Primär-CTA, sticky Mobile, Trust, FAQ/Ohne–Mit, Urgency nur wenn wahr (Notdienst)

### Pass 1 — Structure

Routen, Tokens, Legal-Seiten-Gerüst, ehrliche Inhalte. **Nicht nach Pass 1 shippen.**

### Pass 2 — Watermelon + Furniture

1. Shortlist gegen gebaute IA halten  
2. Install oder Port + **Token-Remap**  
3. Astro-Islands nur wo interaktiv  
4. Dichte: Marketing eher voll — Shelf-Karten mit States, Prozess-Linie, FAQ, sticky CTA ≥44px  
5. Motion-Budget: 1 Hero-Wow + 1 Ambient; Choreografie; reduced-motion  

### Pass 3 — Conversion + Anti-Plain (Pflicht)

Screenshot Desktop-Hero + schwächste Mid + Mobile 390. Fail wenn:

- Hero = Headline + zwei Buttons auf Flat
- Sections = identische Lucide-Grids
- Kein Instrument im ersten Viewport
- 25 %-Zoom nachmittag-leer
- Reskin-Fail **oder** Sibling-Fail

Upgrade bis: erste 3s premium (Material, Tiefe, Instrument im Stillstand lesbar); Conversion klar; Mid hat Signature-Furniture; Copy gesprochen.

### Pass 4 — Polish (wenn Pass 3 „meh“)

Type, optisches Drittel, Marker unter EINEM Nomen, Button shine+spring, List-Stagger, Blur-up, Header-Blur, Fokus, sticky Conversion. Optional ein zweites Micro — keine Küchenspüle.

### Pass 5 — Legal/Security

`legal-security.md`. Keine Tracker „für Wow“ zurückholen.

---

## Quality-Bar (aus QUALITY-BAR, hier operational)

Live-Klasse (Entscheidungen, nie Hex/Copy):

| Site | URL | Stehlen | Nie |
|------|-----|---------|-----|
| Jober | https://jober-a69.pages.dev | Step-Card-Instrument, soft ambient, Marker, Timeline-Node | Blaue Haut, Jobs-Daten |
| Essentialz | https://essentialz-site.pages.dev | Split-Hero, Ohne–Mit, dichte Furniture | Countdown ohne Evidenz; deren Pink/Orange als Default |
| Automater | https://automater.lol | Mesh hinter Typ, Command-Bar als eine Handlung, Stille | Token-Hexes |
| Redesigner | https://redesigner.lol | Marker unter EINEM Nomen, Glow das in Canvas stirbt, Dock, Katalog-Dichte | `#FF2B8A` etc. außer DIESE Marke ist redesigner |

### A. First viewport (≤3s)

Schichten: Canvas → Atmosphere (Blur ≥48–72px) → Vignette in `--bg` → Typ ~38 % Höhe → eine Handlung → Instrument. Header transparent, blur nach ~24px Scroll. Moment mit Werten (Wahrnehmung, Bau, Fallback, RM, Mobile), lesbar im Stillstand.

### B. Dichte

Default **ausgestattet** (7–9); Marketing/Portfolio oft **voll** (11–14) bei echtem Inhalt. Ein Icon-Set, vier Größen, eine Karten-Sprache, Button shine+spring (`scale ~0.955`), sticky ≥44px, States auf Kindern — kein Section-Fade-up-Spam.

### C. Motion

Ein primäres Wow + optional ein Ambient (pause offscreen, Poster). Ein Muster pro Rolle. Kein Lenis unter 768px. overflow-x 0 bei 390. Scroll-CSS nur in `@supports (animation-timeline: view())`.

### D. Nicht Median

Fail ungewählt: Ghost-Brandwort, drei Nomen-Lucide, Pink-Pille auf Schwarz als Identität, Cream+Toy, Fingerprint-Blau/Violett, Inter/Geist-only, Fade-up überall, Dual „Mehr erfahren“, Fake Trusted-by, **oder House-Package**.

---

## Agent-Selbstprompts (zwischen Pässen)

1. **Anti-plain:** „Screenshot Hero + Mid. 5 Plain-Tells. Jedes konkret fixen — keine neuen Seiten.“  
2. **Watermelon:** „Shortlist installieren; remap; echte Inhalte; reduced-motion.“  
3. **Conversion:** „Pfad Hero-CTA → Erfolg. Sackgassen weg; sticky Mobile; Ohne/Mit oder FAQ.“  
4. **Sibling:** „Letzte Skill-Site bei 25 %. ≥3 Achsen wenn zu ähnlich.“  
5. **Class refs:** „jober/essentialz/automater/redesigner — Entscheidungen nicht Hexes. Was fehlt vs. Essentialz-Dichte?“

---

## Pass E — Editorial / Apple-class

Wenn User „plain / nicht modern / nicht premium“ sagt:

- Ein Gedanke pro Chapter, Display `clamp(40px, 8vw, 80px)`, Tracking −0.02…−0.04em, Body ≥17px
- Produkt/Instrument ist Hero; Chrome fast unsichtbar
- Motion expo-out 350–650ms, kein Bounce-Gimmick
- Keine gleichen Card-Grids, kein Glow-Mesh-Spam, keine zwei fetten CTAs

### Font-Paare (eine Paarung, woff2, ≥2 Schnitte Display + 2 Body)

| Mood | Display | Body |
|------|---------|------|
| Apple-adjacent editorial | Inter Tight / Geist | Inter / Geist (17px+) |
| Warm craft / Handwerk | Newsreader oder Instrument Serif | Source Serif 4 oder Literata |
| Tech tool | Satoshi oder Switzer | Inter |
| Luxury | Fraunces **sparsam** ODER Playfair sparsam | DM Sans |

Nie nur system-ui. Taste-Skill warnt: Serif nicht als Autopilot für „premium“ — nur wenn Brief/Marke sie trägt.

### Über-uns

Dieselbe Markenwelt wie Home. Akzent-Tint ok, kein fremdes Blau-Microsite.

---

## Ship-Block

Kein „done“, solange Pass-Log &lt; 3 oder Craft-class 2b fallen würde.  
One-Shot pretty Tailwind ohne Watermelon-Shortlist + Pass 3 = **reject**.
