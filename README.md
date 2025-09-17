# Point code → Route ID & Sequence (GitHub Pages ready)

Een lichte webapp (1 HTML-bestand) waarmee je een **Point code** kunt invullen en in groot lettertype
de bijhorende **Route ID** en **Route sequence** ziet.

- Werkt 100% **client-side** (CSV blijft lokaal in de browser)
- **Android/Chrome-vriendelijk**: file input accepteert alle typen; kies Bestanden → Downloads
- Te hosten op **GitHub Pages** (HTTPS)

## CSV-verwachting
Minimaal deze kolommen:
- `Point code`
- `Route ID`
- `Route sequence`

Andere kolommen in je CSV worden genegeerd.

## CSV laden (3 manieren)
1. **Upload** via de knop (lokaal bestand).
2. **URL-plakken**: geef een publiek bereikbare CSV-URL (HTTPS), bv. een CSV die je samen met `index.html` host.
3. **Automatisch**: als er een `routes.csv` naast `index.html` staat, wordt die automatisch geladen bij openen.

> Let op: dit is **CSV** (platte tekst, komma’s), geen Excel `.xlsx`. Exporteer vanuit Excel/Google Sheets naar CSV.

## Publiceren op GitHub Pages
1. Maak een nieuwe Public repo op GitHub (bv. `pointcode-route-lookup`).
2. Upload `index.html` (en optioneel `routes.csv` in dezelfde map).
3. Ga naar **Settings → Pages** → Source: `Deploy from a branch` → Branch: `main` → Folder: `/ (root)` → Save.
4. Open je Pages-URL: `https://<username>.github.io/pointcode-route-lookup/`.

## Gebruik
1. Laad je CSV (upload of URL of automatisch).
2. Vul je **Point code** in.
3. Klik **Zoek** → de app toont groot: `Route: <Route ID> (seq <Route sequence>)`.
