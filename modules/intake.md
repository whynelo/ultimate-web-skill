# Intake — Tiefen-Briefing / Deep Intake Q&A

**Aufgabe:** Bevor Design oder Code: Fakten sichern, Mode wählen, Legal class setzen.  
**Artefakte:** `BRIEF.md` + `INTAKE.json` (Templates in `templates/`).  
**Prompt:** `prompts/00-intake.md`  
**Überspringen = Fail.**

---

## Wann / When

Jede neue Site, jedes Redesign, jedes Greenfield. Auch wenn der User „mach einfach“ sagt — dann **kurze** Fragen, nicht raten.

---

## Modes (WhyNelo / VERSION-2)

| Mode | Name | Wann |
|------|------|------|
| **1** | Improve in place | Repo existiert. Stack-Idiome halten. Kein reckless Rewrite. |
| **2** | Client redesign | Live-URL anderer Leute. Brand, Fotos, Conversion sind heilig. Audit zuerst. |
| **3** | Greenfield | Keine Live-Site. Median-Landing ist die Gefahr — Lock über-spezifizieren, Sections unter-bauen. |

Default wenn unklar und Broschüre: Mode 3 + Typ A (Astro + Tailwind + Netlify-easy), außer Shop/Auth nachweisbar.

---

## Architektur-Typ A–E

| Typ | Bedeutung | Hosting-Default |
|-----|-----------|-----------------|
| A | Static / Broschüre | Astro + lokale Fonts + Netlify Forms |
| B | CMS | Wie A + CMS; Datenschutz stack-treu |
| C | Auth + DB / SaaS | AGB, Alter ≥16 serverseitig, TOMs |
| D | Payments / Shop | C + Widerruf, Preise/Steuern, ggf. BFSG |
| E | Interaktive KI / UGC | Extra: AI-Act Art. 50 wenn das *Produkt* generiert; DSA/JuSchG-Vorsorge |

---

## Legal class (gleich in Intake locken)

Siehe `modules/legal-security.md`. Eine Klasse: A Info · B Lead · C Account · D Shop · E UGC/18+.

---

## Fragen — dosiert, nicht 40 auf einmal

Runden von 5–8 Fragen. Nach jeder Runde `INTAKE.json` fortschreiben. Stoppen wenn Pflichtfelder stehen.

**Runde 1 — Job**

1. Mode 1 / 2 / 3? Live-URL?
2. Wer zahlt / ruft an? (eine Primär-Persona)
3. Konkrete Angebote (Nomen, die Nutzer suchen) — Liste
4. Eine primäre Handlung (Verb + Nomen)
5. Sprache + Anrede (Du / Sie)
6. Typ A–E und Legal class — Vorschlag machen, bestätigen lassen

**Runde 2 — Heilige Fakten**

7. Rechtsname vs. Marke
8. NAP (Adresse, Tel, Mail) oder `Platzhalter — Anwalt prüfen`
9. Einzugsgebiet / Stunden
10. Echter Beleg (Jahre, Meister, Cases) — nur Evidenz
11. Assets: Logo, Farben, Fotos, Schriften — Herkunft

**Runde 3 — Haltung**

12. Soll sich anfühlen wie: …
13. Darf sich **nicht** anfühlen wie: …
14. Referenzen (URLs, Screenshots) — optional
15. Constraints: a11y-first, reguliert, Kids, Health (HWG)

**Mode 2 extra (Audit vor Pixel):** Rechtsname, IA, Conversion-Pfade, Embeds, Legal-Stand (DDG/TDDDG?), Keep/Improve/Drop/Replace-Tabelle. Nichts erfinden.

---

## Design-Read (eine Zeile)

Nach den Fakten, **bevor** Dials (Phase 1):

> Reading this as: \<page kind\> for \<audience\>, with a \<language\> language, leaning toward \<stack/motion\>.

Beispiel: *„Reading this as: Handwerk-Lead für Hausbesitzer in Köln, mit ruhiger Foto-Leiter, leaning toward Astro + sticky Anruf.“*

---

## Nie erfinden

HRB, USt-IdNr., Reviews, „seit …“, Partnerlogos, User-Counts, Team-Bios, Zertifikate, Countdown-Knappheit.  
Platzhalter sichtbar: `Musterstraße 1, 00000 Stadt` · `TODO: echte Angaben`.

---

## SHARED-CORE (destilliert, WhyNelo)

Pflicht für Client-Redesigns und Greenfield-Broschüren:

1. **Klarheit** — First Seconds: wer, Nomen, eine Handlung.
2. **Hierarchie** — Apple-artig: Content vor Chrome, eine primäre CTA, Typ trägt.
3. **Raum** — Rhythmus als Zahlenfolge, nicht ein `py-24`.
4. **Wow-Budget** — max. ein primäres Wow im ersten Viewport.
5. **Netlify-easy** für Typ A: ein Brand-Config, deutsche README, Drop oder Git.
6. **Echte Assets** vor KI-Bildern; KI nie als echte Mitarbeiter/Jobs.
7. **Conversion behalten** (Mode 2): Tel, Form, WhatsApp, Booking, Shop nicht still droppen.

Vollständige Redesigner-Texte: `modules/redesigner-lol.md`.

---

## Output-Check

`BRIEF.md` ist in ganzen Sätzen lesbar (DE wenn Brief DE).  
`INTAKE.json` valid, keine TBD-Pflichtfelder außer bewusst `unknown` + Begründung.  
Legal class und Typ gesetzt. Design-Read eine Zeile.
