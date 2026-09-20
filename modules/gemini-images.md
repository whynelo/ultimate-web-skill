# Gemini Image Prompts

**Aufgabe:** Bildprompts schreiben, als Datei ablegen, **dem User zeigen**.  
**Phase:** 6 (hart — auch wenn keine Bilder generiert werden)  
**Artefakt:** `GEMINI-IMAGE-PROMPTS.md`  
**Prompt:** `prompts/06-gemini-images.md`

---

## Warum zeigen

Menschen entscheiden über Bildrechte, Marke und „KI-Gesicht: ja/nein“. Stille Prompts im Repo sind ein Skip.

Im Chat:

1. Datei schreiben
2. Inhalt (oder Link/Pfad) **sichtbar** machen
3. Kurz sagen: welche Slots, was *nicht* generiert werden darf

---

## Slots (nur mit Bedarf)

| Slot | Wann | Verboten |
|------|------|----------|
| Hero-Atmosphere | Kein echtes Foto | Fake-Office, Fake-Team, Stock-Handshake als „wir“ |
| Material / Texture | Korn, Papier, Werkstatt, Produktstill | Watermark-Demos, fremde Marks |
| Objekt / Produkt | Object-led Komposition | Hoodie-Kid, Collectible-Demo |
| Section-Plates | Abstrakt oder echte Arbeit | Erfundene Baustellen/Cases |
| Team | Nur wenn User KI-Platzhalter will | Als echte Personen ausgeben |

Default: **echte Fotos >** CSS/SVG **>** KI. KI zuletzt, gelabelt (`KI-Platzhalter` / `AI placeholder`).

---

## Prompt-Handwerk

Jeder Prompt enthält:

- Zweck (wo auf der Site)
- Komposition (Framing, Licht, negativer Raum für Typ)
- Palette **aus DESIGN-SYSTEM** (Hexes nennen)
- Material / Linse / Zeit (nicht „cinematic ultra 8k“)
- Negatives: text glyphs, watermarks, extra fingers, brand logos, readable UI chrome unless requested
- Aspect (16:9 Hero, 4:5 Plate, 1:1 Objekt)

Keine Prompts, die Minderjährige sexualisieren. Keine Prompts, die echte Personen ohne Rechte nachbilden.

---

## Output-Check

- Datei existiert
- User hat sie gesehen (Chat-Zitat oder angehängte Prompts)
- Provenienz-Hinweis fürs README: welche Bilder KI vs. Client vs. Bestand
