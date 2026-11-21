# Misiats Nails – statische Website

Deutschsprachige, mobiloptimierte Website für die Standorte Wuppertal-Langerfeld und Schwelm. Reines HTML, CSS und Vanilla JavaScript; kein Backend, Framework, Cookie, Tracking, Analytics, externes Skript oder eingebettete Karte. Der Buchungsdialog öffnet WhatsApp mit einer lokal im Browser erstellten Terminanfrage.

## Vor dem Livegang noch erforderlich
- **Original-Logo:** In diesem Repository ist derzeit kein originales PNG vorhanden. Das Bild, das im Chat gezeigt wurde, konnte nicht als Datei aus den bereitgestellten Repository-Werkzeugen exportiert werden. `assets/misiats-nails-logo.svg` ist ein neu erstellter Platzhalter und kein unverändertes Original. Bitte laden Sie das Original unter `assets/misiats-nails-logo.png` hoch und ersetzen Sie die Logo-Referenzen in HTML.
- **Fotos:** `photos/*-placeholder.svg` sind eigens erstellte grafische Platzhalter, keine Salon-Fotografien. Bitte ersetzen Sie sie durch freigegebene, helle eigene Fotos: Hero, beide Standortmotive, Langerfeld-Maniküre, Langerfeld-Pediküre, Schwelm-Pediküre sowie die fünf Galerie-Motive (French, Nude, minimalistisches Design, Gel-Lack, Pediküre). Die Platzhalter sind nicht als echte Arbeit/Fotos auszugeben.
- **Schwelm-Preise:** In `js/prices.js` stehen ausdrücklich „Preis auf Anfrage“ – bestätigen und aktualisieren, bevor Preise veröffentlicht werden.
- **Rechtstexte:** `impressum.html` und `datenschutz.html` enthalten genau den gewünschten Hinweis `[Text folgt nach rechtlicher Prüfung]`. Vor Veröffentlichung rechtlich prüfen und vervollständigen lassen.
- **Sprachen:** EN und UA sind als Auswahl vorbereitet, die Zielseiten sind noch nicht übersetzt/angelegt.

## Angaben aktuell
- Wuppertal-Langerfeld: Spitzenstraße 30, 42389 Wuppertal (Maniküre und Pediküre)
- Schwelm: Wilhelmstraße 10, 58332 Schwelm (nur Pediküre; vom Inhaber zuletzt im Chat bestätigt)
- Öffnungszeiten laut Angabe: Montag bis Samstag, 10:00–20:00 Uhr
- WhatsApp: +49 172 6127991

## Preise ändern
Alle Preise zentral in `js/prices.js` bearbeiten. Kategorien sind `langerfeld.manicure`, `langerfeld.pedicure` und `schwelm.pedicure`. Preisangaben vor Veröffentlichung durch den Inhaber bestätigen.

## WhatsApp-Nummer ändern
`js/main.js`: in der URL `https://wa.me/491726127991` die Nummer im internationalen Format ohne `+`, Leerzeichen oder führende Null eintragen. Formularfelder werden nicht auf einem Server gespeichert oder übermittelt. WhatsApp öffnet sich erst nach dem Absenden; die Bestätigung erfolgt persönlich.

## Fotos und Logo ändern
Dateien in `photos/` und `assets/` austauschen und bei Bedarf `src` in den HTML-Dateien ändern. Für Performance eigene WebP/JPEG-Bilder passend zuschneiden und komprimieren; das Originalbild nicht ohne Erlaubnis verwenden. Platzhalter-SVGs liegen unter aussagekräftigen `*-placeholder.svg` Namen.

## Lokal ansehen
Einfach `index.html` in einem Browser öffnen oder einen lokalen statischen Server verwenden, zum Beispiel `python3 -m http.server 8000`, dann `http://localhost:8000` aufrufen.

## GitHub Pages veröffentlichen
1. Änderungen nach `main` pushen.
2. GitHub-Repository → **Settings → Pages** öffnen.
3. Unter Build and deployment **Deploy from a branch** wählen, Branch `main`, Ordner `/(root)` und speichern.
4. Nach erfolgreicher Bereitstellung die von GitHub angezeigte Pages-Adresse prüfen. `sitemap.xml` und `robots.txt` sind auf `https://hasibhasib12.github.io/Misiats-nails/` eingestellt; falls die Veröffentlichungsadresse abweicht, beide Dateien aktualisieren. Netlify kann das Repository ebenfalls als statische Root-Site veröffentlichen.

## Barrierefreiheit und Datenschutz
Semantische Bereiche, Tastatur-bedienbares Menü und Lightbox, Bild-Alternativtexte, responsives Layout und Fokuszustände sind vorgesehen. Die Website setzt keine Cookies, kein Tracking und keine Analyse ein. Die externe Google-Maps-Verknüpfung wird nur bei Klick aufgerufen; sie ist keine eingebettete Karte. Bitte vor Livegang auch Kontrast, Tastaturbedienung und Rechtstexte prüfen.
