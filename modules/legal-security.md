# Legal + Security — DE / EU (hartes Modul, immer)

**Status:** Operative Checkliste für Agenten. **Kein Rechtsrat.**  
**Always-on:** Jeder Lauf lädt dieses Modul, unabhängig von Phase.  
Adaptiert aus redesigner-jev `LEGAL-SECURITY.md`.

Keine Garantie „unverklagbar“. Shop, Accounts, Zahlung, UGC, Health, Kids, Glücksspiel → **Anwalt vor Live-Traffic**. README braucht `## Lawyer review`, wenn Risiko > Info-Site.

Normen (Recherche-Stand 2026-09): **DSGVO**, **BDSG**, **DDG** (§ 5 Impressum; TMG ersetzt), **TDDDG** (§ 25 Endgeräte), **UWG**, **BFSG** (elektronischer Geschäftsverkehr ab 2025-06-28), **DSA** / JuSchG, **BGB** (Fernabsatz / Widerruf / Geschäftsfähigkeit).

---

## 0) Site-Klasse (Lock / Legal)

In `DESIGN-SYSTEM.md` → `## Legal class` genau eine Klasse:

| Klasse | Beispiele | Pflicht-Minimum |
|--------|-----------|-----------------|
| **A — Info / Portfolio** | Visitenkarte, Agency, Portfolio ohne Checkout | Impressum, Datenschutz, HTTPS, datensparsam |
| **B — Lead / Kontakt** | Formulare, Newsletter | A + Zweckbindung, Spam-Schutz, Fristen, DOI Newsletter |
| **C — Account / SaaS** | Login, Credits | B + AGB, AVV, Art.-8-Alter, Art. 15–21, TOMs, Logging |
| **D — Shop / Fernabsatz** | Checkout | C + Widerruf, Pflichtinfos, Preise/Steuern, ggf. BFSG |
| **E — UGC / Plattform / 18+** | Uploads, Feeds | D-Risiko + DSA/JuSchG, Moderation, ggf. AV-System |

Ship ohne Klasse + Checkliste = **fail Legal**.

---

## 1) Impressum (§ 5 DDG)

Footer + eigene Seite, **max. 2 Klicks**.

Typisch: Klarname/Firma, ladungsfähige Anschrift (kein P.O. Box allein), E-Mail, ggf. Telefon, bei GmbH Registergericht/HRB/Vertretung, USt-IdNr. falls vorhanden, ggf. Aufsicht/Beruf.

Platzhalter nur mit `TODO: echte Angaben` — **nie erfundene HRB/USt**. Label **DDG**, nicht TMG.  
Social-Profile: Link zum Impressum der Website.

---

## 2) Datenschutz (Art. 13/14 DSGVO)

Eigene Seite, **stack-treu**.

Bausteine: Verantwortlicher (+ DSB), Zwecke + Rechtsgrundlagen, Kategorien/Empfänger/Drittland/SCCs, Speicherdauer, Rechte inkl. Aufsicht, Pflicht vs. freiwillig, Profiling falls ja, Cookies/localStorage + Verweis.

**Craft-Default:** lokale Fonts; kein GA/Meta/Hotjar ohne Consent+AVV; Analytics privacy-first oder keine; Embeds als Facade.

---

## 3) Cookies / Tracking (§ 25 TDDDG)

- Technisch notwendig (Session, Warenkorb, Consent-Log, CSRF): kein Banner.
- Alles andere: Einwilligung **vor** Laden.
- Banner falls nötig: Ablehnen = Akzeptieren auf Ebene 1, keine Dark Patterns, Footer-Widerruf.
- Einwilligung dokumentieren.
- **Bevorzugt: Architektur ohne Banner.**

---

## 4) Formulare & Newsletter

Nötige Felder, Labels, Fehler. Kontakt: Zweck + Datenschutz-Link — keine Fake-„Ich willige in alles ein“-Pflicht für bloßen Versand. Newsletter: **Double-Opt-In**. Honeypot/Rate-Limit. Keine Webhooks ohne AVV-Klarheit.

---

## 5) Alter

### DSGVO Art. 8
Deutschland: **16**. Unter 16: elterliche Verantwortung + angemessene Vergewisserung — wenn Verarbeitung auf Einwilligung beruht und der Dienst sich (auch) an Kinder richtet.

### Default Klasse C/D
1. Registrierung: Geburtsdatum oder klare „mindestens 16“ — besser Geburtsdatum, **serverseitig**.
2. Zahlung / verbindliche Verträge / Credits: zusätzlich **18** (Geschäftsfähigkeit) oder dokumentierter Eltern-Flow (Anwalt).
3. Unter Mindestalter: ablehnen oder eingeschränkt + Consent-Pfad (nicht nur Checkbox).
4. Kids-Angebot: kindgerechte Sprache. Kein Marketing-Profiling von Kindern.

### 18+ / UGC
Schwere Jugendgefährdung: geschlossene Gruppe + anerkanntes AV-System, nicht nur „Ich bin 18“. Plattformen: DSA Art. 28 / JuSchG — Extra-Scope.

### Agent nie
Minderjährige stillschweigend · Accept-all als einzige Option · Alterscheck nur Client.

---

## 6) AGB, Widerruf, Preise (C/D)

AGB vor Vertrag (Checkbox+Link, nicht vorausgefüllt). Shop: Widerruf + Muster, Lieferung/Zahlung, Preise inkl. Steuer. Digitale Sofort-Inhalte: Sonderregeln (Anwalt). Credits: Wesen, Verfall, kein versteckter Abo-Zwang.

Typ D extra (Redesigner legal-de): § 312j, PAngV, Widerrufsbutton § 356a wo einschlägig, Dauerschuld Kündigungsbutton § 312k.

---

## 7) Auftragsverarbeitung & Drittland

README `## Processors`: Hosting, Auth, Mail, Payment, AI, Storage.  
Pro EU-relevantem Prozessor: AVV Art. 28 + Transfer. Ohne Status → Lawyer-TODO.

---

## 8) BFSG

Seit 2025-06-28 oft B2C E-Commerce. Kleinstunternehmen (&lt;10 MA und ≤2 Mio. €) bei Dienstleistungen oft ausgenommen — in README begründen.  
Betroffen: EN 301 549 / WCAG-Richtung, Erklärung, Tastatur, Kontrast, Labels, Fokus.

Skill verlangt **immer** a11y-Baseline.

---

## 9) Security (ship-blocking)

| Kontrolle | Pflicht |
|-----------|---------|
| HTTPS | ja |
| Secrets nur Server/Env | ja |
| Headers: CSP-Start, Referrer-Policy, X-Content-Type-Options | ja |
| Auth: Hash/IdP, Session, CSRF | ja bei Accounts |
| Uploads: Typ/Größe/Scan-Pfad | ja bei Upload |
| Rate limits Login/Form/API | ja |
| `pnpm audit` / gleich — kritische Fixes | ja |
| Admin/Debug aus Prod | ja |
| Logs ohne Secrets / PAN / Tokens | ja |
| Backup + Incident-Hinweis | Klasse C+ |

AI-Keys nur Server. EU-AI-Act Art. 50 nur wenn das **Produkt** Chatbot/Generator/Deepfake ist — kein Badge „mit KI gebaut“, weil ein Agent HTML schrieb.

---

## 10) Footer

Immer: Impressum, Datenschutz, Kontakt. Optional: AGB, Widerruf, Cookies, Barrierefreiheit.  
Copy: Du/Sie wie Site. Keine leeren „wir nehmen Datenschutz ernst“-Essays.

---

## 11) Agent-Workflow (in Phase 5 Schritt Legal + Phase 7/8)

1. Legal class setzen  
2. Stack-Inventar  
3. Seiten bauen  
4. Tracker weg oder hinter Consent  
5. Forms  
6. Auth-Alter  
7. Processors + AVV-TODOs  
8. Headers + Secret-Scan  
9. Network-Tab  
10. Review-Gate  

**Ship blocked:** fehlendes Impressum/Datenschutz; Tracker ohne Consent; erfundene Registerdaten; Accounts ohne Alter (C+); Secrets im Client.

---

## 12) Disclaimer (jede README)

> Diese Checkliste ersetzt keine Rechtsberatung. Abmahnungen und Aufsichtspraxis ändern sich. Vor kostenpflichtigem Traffic oder sensiblen Daten: Anwalt gegenlesen lassen.

Kein Link zur abgeschalteten EU-ODR-Plattform.
