# Natürlich Abgesichert — Pferd- und Reitsport-Landingpages

Drei zielgruppen-spezifische Landingpages plus eine Hub-Seite für den
Pferd- und Reitsport-Bereich von **Natürlich Abgesichert**
(Inhaber: Otto Boldt, Leipzig).

## Inhalt

```
.
├── hub/index.html                  → Übersichts-Seite mit 3 Zielgruppen-Auswahl
├── landingpage.html                → Pensionsstall + Haltergemeinschaft
├── index.html                      → Weiterleitung zur landingpage.html
├── verkaufsstall/index.html        → Verkaufs- + Beritt- + Aufzuchtbetriebe
├── berufsreiter/index.html         → Berufsreiter + Reitlehrer
└── CLAUDE-START-HIER.md            → Anleitung für Review per Claude Code
```

## Lokale Vorschau

Mit beliebigem statischem Server starten, z. B.:

```bash
# Python:
python -m http.server 8765

# Oder PHP:
php -S 127.0.0.1:8765

# Oder Node:
npx http-server -p 8765
```

Dann im Browser öffnen:

- `http://localhost:8765/hub/` — Übersicht
- `http://localhost:8765/landingpage.html` — Pensionsstall
- `http://localhost:8765/verkaufsstall/` — Verkauf/Beritt/Aufzucht
- `http://localhost:8765/berufsreiter/` — Berufsreiter/Reitlehrer

## Tech-Stack

- Pure HTML + CSS + JS (kein Framework)
- Royal-Palette (Königsblau-Violett #2D2A6B, Gold #B89A5C) + Georgia-Serifenschrift
- Responsive, mobile-first
- Externe Abhängigkeiten:
  - Otto-Foto vom natuerlichabgesichert.de-CDN
  - Pferd-Fotos von Unsplash + Pferdefotos der natuerlichabgesichert.de-Mediathek
  - Calendly Popup-Widget (`assets.calendly.com`)
  - WhatsApp Deeplinks (`wa.me`)

## Platzhalter (vor Live-Schaltung ersetzen)

- `49XXXXXXXXXX` — WhatsApp-Nummer
- `[CALENDLY-USERNAME]/beratung` — Calendly-Buchungs-URL
- `[Versicherungsmakler nach §34d Abs. 1 GewO]` — Status
- `[D-XXXX-XXXX-XX]` — Vermittlerregister-Nummer

## Status

Vorschau-Versionen, noch nicht live deployed.

---

© 2026 Natürlich Abgesichert · Inhaber Otto Boldt
