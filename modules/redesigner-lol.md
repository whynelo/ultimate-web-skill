# Redesigner.lol + WhyNelo SHARED-CORE / VERSION-2

**Aufgabe:** Redesigner-Methode, Quellen-Disziplin, Apple-HIG-artige Prinzipien, Modes.  
**Phasen:** Wissen immer; Bau-Schritte 01–07 **innerhalb** Phase 5, nachdem 0–4 Artefakte existieren.  
**Upstream:** https://redesigner.lol/prompts · https://redesigner.lol/quellen  
Paraphrase der Regeln. Keine 45-kB-Kleister, keine bezahlten Packs rekonstruieren.

---

## Der Lauf (warum kurz)

Lange Pastes erzeugen Agency-Median (Lost in the Middle). Subtraktion allein erzeugt Nachmittag-leer. Deshalb: kurze Schritte, Tokens oben, Ausstattung als eigener Schritt.

Redesigner-Schritte (Phase 5):

| # | Name | Tut |
|---|------|-----|
| 01 | Lock | Nur DESIGN/DESIGN-SYSTEM Werte — hier meist schon aus Phase 1–3. Lücken schließen, STOP. |
| 02 | Viewport | Nur erste Fläche, Schichten, Moment |
| 03 | Rest | IA der Komposition, Hero steht |
| 04 | Ausstattung | Bausteine mit Werten, ein Icon-Set, Choreografie |
| 05 | Texte | Deutsch gesprochen, Überschrift ≠ erster Satz |
| 06 | Anti-Slop | Median **und** Nachmittag; ab 4 Treffern neu |
| 07 | Legal | Echter Stack (`legal-security.md`) |

Ein Chat, ein Schritt, STOP. Quellen erst **nach** Lock, ein Rezept pro Paste, Skin aus Tokens.

---

## Acht Lock-Entscheidungen (Werte, nicht Stimmung)

1. Typ A–E  
2. Komposition + Viewport-Schichten hinten→vorne  
3. Gitter als **Verhältnis** (7/5, 8/4, Marginalie+42rem) — nicht 1/1 dreimal  
4. Typo-Skala Tabelle, clamp, 1.2–1.5, Maß 45–75ch, Gewichtssprung ≥300, lokal woff2  
5. Palette Hex + Akzent-Budget — keine Fingerprint-Hexes  
6. Rhythmus-Folge (nicht ein `py-24`)  
7. Ein Signatur-Moment: Wahrnehmung, Bau, Fallback, reduced-motion, Handy + Material  
8. Ausbau still / ausgestattet / voll + Bausteine, EIN Icon-Set, EINE Karten-Sprache, Cut-Liste  

Job des ersten Viewports: wer, konkretes Nomen, eine Handlung.

---

## Viewport-Handwerk (02)

- `--bg` volle Höhe (100dvh / min 88dvh), kein Section-Border der die Fläche schneidet  
- Eine Material/Medium-Ebene aus dem Lock  
- Vignette/Scrim in die Canvas, keine harte Horizont-Kante  
- H1 Versprechen, clamp, `text-wrap: balance`, 16–18ch; ein Fakt darunter  
- Eine Handlung ≥44px; kein zweiter Ghost; Text-Link sekundär ok  
- Moment gebaut  
- Typ ~38 % Höhe, nicht totzentriert  
- Header transparent  
- Micro 50–200ms; ein Live-Medium max; Poster im HTML; `pointer-events: none` auf Deko  
- Ghost-Typ hinter Medien opacity 0.05–0.07 oder weglassen  
- Handy: overflow-x 0, H1 lieber drei Zeilen als Schrumpfen, eine sticky Handlung  

---

## Ausstattung (04) — gegen Nachmittag

ContentCut / Univelop / Apple Store sind dicht und trotzdem nicht KI, weil jeder Block echten Inhalt hat und **ein** Bewegungsmuster pro Rolle.

Reihenfolge: Icon-Set (Lucide/Phosphor/Tabler/Iconoir — ein Set, 1.5px, Größen 0.8/1.1/1.5/2rem) → eine Karten-Sprache → gelockte Blöcke mit Werten → Choreografie auf Kindern → kleine Assets.

Nur echter Beleg. Fehlt Inhalt: streichen oder „Foto folgt“. Nie erfinden.

---

## Copy-de (05)

Anrede aus Lock, Sentence Case. H1 konkret. Erster Satz wiederholt die H1 nicht. Buttons Verb+Nomen, ein Primär-CTA wortgleich. Zahlen nur belegt.

Verboten (Reskin-Killer): Willkommen auf unserer Website; leidenschaftliches Team; ganzheitliche/innovative Lösungen; Entdecken Sie das volle Potenzial; Mehr erfahren als Haupt-CTA; unlock/unleash/seamless/next-gen; Gedankenstrich-Regen; Title Case auf Buttons; Copy die nach Namens-Tausch für jede Agentur gilt.

---

## Anti-Slop (06) — beide Richtungen

**Nachmittag:** keine Icons · keine Karten-Sprache · kein Beleg obwohl möglich · kein FAQ/Ablauf/Ansprechpartner · keine States · eine Animation, Rest PDF · &lt;8 Sections obwohl Inhalt da · Bilder ohne Blur-up/Caption/aspect · Header ohne Scroll-Verhalten · keine sticky Mobile-Handlung.

**Median:** Ghost-Wort · drei Leistungsnomen · Cream+Toy · Pink-Pille auf Schwarz als ganzes Design · austauschbare Copy.

**Klassiker:** Fingerprint-Akzent · Inter/Geist-only · Badge+H1+Absatz+Ghost · genau drei Icon-Karten · Bento-as-features · cream-italic ungewählt · zinc-950+Glow · Sparkle/Rakete · FAQ-Paraphrase · Fake Trusted-by · Lenis global · Fade-up jede Section · `lang=en` bei DE · Overflow · zwei Autoplay-Medien · Horizont an Border abgeschnitten · scharfe Neon-Kugel · Demo-Headlines live.

Kompositions-Treffer wiegt schwerer. Ab 4 gesamt: Lock/Viewport neu, kein Feinschliff.

---

## SHARED-CORE (WhyNelo, destilliert)

Öffentliche HIG-Idee + Studio-Praxis, nicht Apples Branding klonen:

| Prinzip | Praxis |
|---------|--------|
| Clarity | First seconds lesbar, eine Handlung, Kontrast |
| Deference | UI dient Inhalt; Chrome tritt zurück |
| Depth | Schichten und Motion erklären Hierarchie, nicht dekorieren |
| Consistency | Ein Token-System, eine Karten-Sprache, ein Icon-Set |
| Accessibility | Fokus, 44px, reduced-motion, Semantik — von Tag 1 |
| Privacy | Datensparsam, Consent vor Tracker |
| Craft | Unfertiges Detail = unzuverlässiges Produkt |
| Delight | Persönlichkeit stützt die Aufgabe |

Netlify-easy Typ A: `netlify.toml`, eine Brand-Config, deutsche README, NAP zentral.

---

## VERSION-2 — Client redesign (Mode 2)

1. **Deep audit** der Live-URL vor Build: Name, NAP, IA, Conversion, Embeds, Trust nur evident, Legal-Stand, Tech-Smells, Assets, Keep/Improve/Drop/Replace.  
2. Kernfunktionen halten. Typ A default außer Shop/Auth evident.  
3. Assets: Client → Bestand → sachliche Listing-Fotos → CSS/SVG → KI zuletzt, gelabelt.  
4. Legal für das echte Business; Shop-Pflichten nicht „vergessen“.  
5. SEO: Titles, Semantik, LocalBusiness JSON-LD wenn NAP wahr.  
6. Kein Competitor-Pixelclone.

Mode 1: vom existierenden Stack aus; Must-Keep-Inventar; ein Token-System; kein Feature-Creep.  
Mode 3: Lock über-spezifizieren; Sections ohne Inhalt streichen; Median-IA (Hero→3 Cards→Bento→FAQ) verboten wenn eine Komposition gelockt ist.

---

## Kompositions-Archetypen (eine)

Stilles Feld · Asymmetrischer Split · Satzspiegel · Foto-Leiter · Spec-Sheet · Objekt-Bühne · Plakat · Verzeichnis · Kino-Sequenz · Theke.

Converting B2B/Foto-Landing: Spine Promise → Proof → Problem → Offer → Method → Objections → dieselbe CTA. Architektur studieren, nicht klonen. Health: HWG.

---

## Quellen-Disziplin (/quellen)

Rezept **nach** 01. Preview, Umbau, Skin aus DESIGN. Nie Rezept + Ultimate + Lock in einem Paste.

Kategorien (URLs auf der Quellen-Seite, nicht hier 110 Einträge wiederholen):

- Prompt-Bibliotheken: MotionSites (nur FREE), Meez, anti-slop-website-prompts, …  
- Komponenten: 21st.dev, Icon-Sets, Rough Notation (unter EINEM Nomen), Shots.so, Aceternity/Magic UI/React Bits als Rezept  
- Motion/Assets: Unicorn, ShaderGradient, Rive community, Lottie (Runtime self-host), Spline nur object-led, GSAP eine Timeline, Motion, Haikei/fffuel  
- Galerien: Godly (Phase 2 Pflicht), Awwwards, ContentCut/Univelop/Apple Store als Klasse, Refero, Hoverstat.es, Brutalist, Minimal Gallery  
- Anti-Slop-Listen: signs-of-ai-design, Sailop, impeccable.style/slop  
- Type: Hallmark, Fontshare (download + host), Fontsource, Utopia clamp mit Mobile-Max  

**Klasse ContentCut:** zweischichtige Glaskarte, 120s-Logo-Band, Ergebnis-Karten, Ohne/Mit, Shine-Button, Rive sparsam, Ansprechpartner — Countdown/Lenis draußen.  
**Univelop:** Marker unter einem Wort, echte Funktions-Kacheln, Heute/Mit, Schritte mit Tags, Blur-up, Zitat-Regal.  
**Apple Store:** Regal-Scroller Snap+Paddle, eine Karten-Sprache, zweiteilige Überschrift — kein SF als Identität.

MotionSites/Meez: nur FREE; Demo-Skin strippen; ein Wow; ghost type lesbar; Decision-Log in README.

---

## Extra-Rezepte (nach Lock, nicht statt Pipeline)

- **Methode:** Klasse redesigner.lol = eine Primitive, ein Feld, eine Handlung, ein Moment — nicht deren Tokens.  
- **Runtime-Feld:** stilles Tool, Ambient-Ellipsen blur ≥72px, Dock ≠ Chat.  
- **Local-Fachbetrieb:** Foto der Arbeit oder type-led, Definitionsliste, sticky Call, zentrale NAP-Config.  
- **Subtle motion:** Budget hart; CSS first; Mobile-Fails (Lenis, zwei WebGL, Marquee-Overflow) vermeiden.

---

## Klasse vs. Clone

Seite in der Klasse von redesigner.lol: Methode, nicht Clone. Eigene Hexes. Tokens von redesigner nicht stehlen.
