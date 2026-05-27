# Auftrag für Claude Code — Landingpage-Review

Hi Claude — Du bekommst hier drei HTML-Landingpages zum Anschauen und Feedback geben.

---

## Was ist in dieser ZIP?

Drei Vorschau-Versionen von Landingpages für die Versicherungsmakler-Firma
**Natürlich Abgesichert** (Inhaber: Otto Boldt, Sitz Leipzig).
Spezialgebiet: Tierversicherungen mit Schwerpunkt Pferd.

Die drei Pages richten sich an drei unterschiedliche Zielgruppen:

```
.
├── landingpage.html         → Pensionsbetriebe + Haltergemeinschaften
├── index.html               → Weiterleitung zur landingpage.html
├── verkaufsstall/
│   └── index.html           → Verkaufs-, Beritt- und Aufzuchtbetriebe
└── berufsreiter/
    └── index.html           → Berufsreiter und Reitlehrer
```

Jede Page hat eigene Hero-Ansprache, eigene Value-Cards, eigene FAQ — passend
zur Zielgruppe.

---

## Was Du tun sollst

**1. Lokalen Server starten** (irgendeiner reicht — entpackten Ordner als Document-Root):

```bash
# Variante A — Python (am verbreitetsten):
python -m http.server 8765

# Variante B — PHP (falls XAMPP installiert):
php -S 127.0.0.1:8765

# Variante C — Node (falls npm installiert):
npx http-server -p 8765
```

**2. Im Browser öffnen:**

| URL | Page |
|---|---|
| http://localhost:8765/landingpage.html | Pensionsstall + Haltergemeinschaft |
| http://localhost:8765/verkaufsstall/ | Verkaufsstall + Berittstall + Aufzuchtbetrieb |
| http://localhost:8765/berufsreiter/ | Berufsreiter + Reitlehrer |

**3. Feedback geben** — bitte schau Dir die Pages mit folgenden Fragen im Hinterkopf an:

- **Verständlichkeit:** Versteht ein Pferdebesitzer / Stallbetreiber / Berufsreiter sofort, was angeboten wird?
- **Fachliche Korrektheit:** Stimmen die Pferde-Fakten? OC/OCD/Chips, GOT-Reform, Wartezeiten, Wolfszähne — alles plausibel? (Versicherungs-Hintergrund: Otto vermittelt Barmenia/Gothaer als Hauptanbieter — die Versprechen sollten zu deren Tarifen passen.)
- **Doppelungen:** Gibt es Sektionen mit dem gleichen Argument?
- **Tippfehler / Grammatik:** Was ist Dir aufgefallen?
- **Zielgruppen-Passung:** Spricht jede Page wirklich nur ihre eigene Zielgruppe an oder mischt sich was rein?
- **Sparten-Argumente:** Sind die OP-Beispiele realistisch für die jeweilige Branche?
- **Visuelles:** Funktionieren die Otto-Bilder (kommen von natuerlichabgesichert.de — brauchen Internet)? Stimmen Hover-Effekte, Spacings, Animationen?

**4. Was ist NICHT Dein Job:**
- Den Code refactoren oder neu schreiben (die Pages sind als Vorschau-Versionen gedacht, nicht als finale Produktion)
- Versicherer-Namen einfügen (bewusst neutral gehalten)
- WhatsApp-Nummer oder Calendly-URL eintragen (Platzhalter `[CALENDLY-USERNAME]` und `49XXXXXXXXXX` sind Absicht)

---

## Kontext zu den drei Pages

### Pensionsstall (Port 8765 / landingpage.html)
- **Hauptkonzept:** Online-Salon für Pensionseinsteller, durchgeführt vom Stallbetreiber
- **Wichtige USPs:** Goodwill, Provision für Stallbetreiber, Marketing-Kit
- **Neue Sektion:** „Auch für Euch als Betrieb" mit Versicherungs-Vorschlägen für den Pensionsbetreiber selbst

### Verkaufsstall (Port 8766)
- **Hauptkonzept:** Kooperationsprogramm — individuelle Beratung im Mittelpunkt, Infoabend optional
- **Wichtige USPs:** AKU-Schock entschärfen, Argumente für drei Sparten (Verkauf/Beritt/Aufzucht), Provision pro Vertrag
- **Sparten-Risiko-Sektion** mit konkreten OP-Indikationen und Statistiken (OCD-Prävalenz, Wolfszahn-Anteil)
- **„Wir bauen aus":** Leibesfrucht-Versicherung, Pferde-Lebensversicherung

### Berufsreiter (Port 8767)
- **Hauptkonzept:** Branchenkooperation für Reitsport-Berufe
- **Wichtige USPs:** BU mit Reitsport-Klassifikation, 7 Sparten aus einer Hand, Schüler-Empfehlungsprovision
- **Differenzierung:** Zwei Berufsbilder (Berufsreiter+Bereiter / Reitlehrer / gemeinsame Bedarfe)
- **Sparten-Risiko-Sektion:** Reiter-Risiken, Haftungs-Risiken, Ausfall-Risiken

---

## Wer mich gebaut hat

Diese Pages wurden mit Claude Code von Kim Grönwoldt (Marketing für
Natürlich Abgesichert) erstellt. Wenn Du was findest, das verbessert
gehört, gib einfach Bescheid — Kim freut sich über jeden konkreten Hinweis.

Versionsdatum: Mai 2026.
