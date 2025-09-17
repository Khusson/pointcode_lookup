# Point code → Route ID & Sequence (Android-vriendelijke upload + BE/leading zeros optioneel)

Deze versie maakt het eenvoudiger op Android om een CSV uit **Bestanden/Downloads** te kiezen en laat toe om
**Point codes in te geven zonder 'BE' en zonder voorloopnullen** (bijv. `25833` matcht `BE025833`).

## CSV-verwachting
Minimaal deze kolommen:
- `Point code`
- `Route ID`
- `Route sequence`

## CSV laden
- **Upload** (brede accept-lijst: `.csv,text/csv,application/csv,...,*/*`) → Android toont Bestanden/Downloads.
- **URL**: plak een publiek bereikbare CSV-URL (HTTPS).
- **Automatisch**: `routes.csv` naast `index.html` wordt geladen als die bestaat.

## Gebruik
1. Laad je CSV.
2. Vul je **Point code** in — met of zonder `BE` en voorloopnullen (bv. `BE025833` = `25833`).
3. Klik **Zoek** → je ziet groot: `Route: <Route ID> (seq <Route sequence>)`.

## Publiceren op GitHub Pages
Upload `index.html` (en optioneel `routes.csv`) in de root van een public repo en activeer Pages (Deploy from a branch → main → root).
