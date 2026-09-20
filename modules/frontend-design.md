# Frontend-design — Purpose → Aesthetic → Craft

**Aufgabe:** Bevor Code: Zweck, Ästhetik, dann Type / Color / Composition / Interaction.  
**Phase:** 1  
**Upstream:** Anthropic frontend-design  
https://github.com/anthropics/skills/tree/main/skills/frontend-design  
https://claude.com/blog/improving-frontend-design-through-skills

Paraphrase der **Methode**. Kein Wholesale des copyrighted SKILL-Texts.

---

## Prozess / Process (Contract)

1. **Purpose** — Welches Problem löst die Fläche? Wer handelt in 3 Sekunden?
2. **Aesthetic** — Eine gerichtete Haltung (nicht „modern clean“). Risiko, das zum Brief gehört.
3. **Typography** — Paarung mit Charakter; Skala; Maß. Type ist Design, nicht Carrier.
4. **Color** — 4–6 benannte Hexes, dominant + scharfer Akzent. CSS-Variablen.
5. **Composition** — Konzept in einem Satz + grobes ASCII. Ausrichtung bewusst.
6. **Interaction** — Welche eine Bewegung antwortet auf den Menschen? Rest ruhig.
7. **Review gegen Brief** — Liest sich der Plan wie der Default für *jede* ähnliche Seite? Dann ändern und begründen.
8. **Erst dann Code.**

Das ist kompatibel mit Redesigner-Lock (acht Entscheidungen) — frontend-design liefert die *Begründung*, Lock die *Werte*.

---

## Subject matter first

Branche, Materialien, Vernakular steuern die Optik. Spielzeug ≠ Analysten-Dashboard.  
Echten Inhalt des Briefs durchziehen — nicht Generic-SaaS-Copy auf beliebiges Gewerk.

Hero = das Charakteristischste der Welt des Subjekts (Headline, Foto, Instrument, Demo) — nicht automatisch Big-Number + Gradient.

---

## Kalibrierung: Cluster meiden (wenn der Brief sie nicht verlangt)

Aktuelle AI-Cluster (legitim *nur* wenn der Brief sie pinnt):

- Warm cream + Serif + Terracotta/Clay
- Near-black + Acid-Grün oder Zinnober
- Broadsheet: Hairlines, radius 0, Zeitungs-Spalten
- SaaS-Card-Kit: gleiche Cards, ein Radius, weicher Grauschatten, Deko-Wash
- Template-Chrome: ALL-CAPS-Eyebrow überall, Middle-Dots, „WORD — fragment“, Fake-Black `#0B0B0B`, Mono-Labels, `→` an jedem Button

WhyNelo-House (void + Acid + Magenta + Dual-Orbs) ist **zusätzlich** gebannt — `modules/differentiation.md`.

---

## Restraint

Mut an **einer** Stelle. Umgebung diszipliniert. Ein Accessoire entfernen (Chanel-Regel).  
Qualität unsichtbar: 390px, Fokus, reduced-motion, Kontrast. Nicht als Badge „a11y“ verkaufen.

Motion: nicht-user-getriggert sparsam. Eine orchestrierte Sequenz schlägt Fade-up auf jeder Section. Antwort auf Klick/Expand ist willkommen.

---

## Copy als Design

Worte existieren, damit man handelt. Nutzer-Sprache, Aktiv, Sentence Case.  
CTA sagt was passiert. Gleicher Name durch den Flow. Empty/Error = Richtung, kein Mood.  
DE: gesprochen, siehe Redesigner Copy-Regeln in `redesigner-lol.md`.

---

## Output in DESIGN-SYSTEM.md

```
## Frontend-design
- purpose:
- aesthetic: (extrem, wahrhaftig)
- type_rationale:
- color_rationale:
- composition_ascii: (klein)
- interaction_one_liner:
- uniqueness_check: was am Plan nicht der Cluster-Default ist
```
