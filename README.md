# C-HAWQ Residential Canal Dashboard

An interactive map of Florida's statewide residential canal footprint — 3,050 mapped canal systems. Filter by county, city/municipality, water management district, basin planning unit, and canal size; click any canal for its full attributes; recolor canals, switch to satellite imagery, and export selections as Shapefile, GeoJSON, or CSV.

Built and maintained by **C-HAWQ — the Coastal Habitat and Water Quality Initiative**.

## Live site

Once GitHub Pages is enabled (Settings → Pages → Deploy from a branch → `main` / root), the dashboard is live at:

`https://<account>.github.io/<repo>/`

## What's in this repo

- **index.html** — the entire dashboard. The canal data is embedded in this one file, so there's nothing else to serve.

## Using it

Open the live link in any modern browser. An internet connection is required — the map libraries, fonts, basemap tiles, and the C-HAWQ logo load from the web. The page explains its own controls: filter with the dropdowns or by clicking a chart bar, click a canal for details and to add it to an export set, recolor from the legend, and download from the Export menu.

To preview locally, serve the folder over HTTP (`python -m http.server`) and open `index.html` — double-clicking the file won't work, because browsers block local file reads.

## Data

Each polygon is one mapped residential canal system with its area, perimeter, county, city/municipality, water management district, basin planning unit, HUC-8, and WBID. The footprint is derived from C-HAWQ's canal delineation pipeline, building on public sources (U.S. Geological Survey National Hydrography Dataset; Florida Department of Environmental Protection basin data; Florida city-limits data). City assignment is a spatial join to 2021 Florida municipal boundaries.

## License

Code © 2026 C-HAWQ. All rights reserved. The dashboard data is released under Creative Commons Attribution–NonCommercial–NoDerivatives 4.0 (CC BY-NC-ND 4.0). See [LICENSE](LICENSE) for details and for the terms covering the underlying public data.

## Contact

Nathan — nathan@chawq.org
