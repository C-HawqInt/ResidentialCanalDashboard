# C-HAWQ Residential Canal Dashboard

An interactive map of Florida's statewide residential canal footprint. Filter by county, city/municipality, water management district, basin planning unit, canal size, form, receiving waters, and connectivity; click any canal for its full source attributes; recolor canals, switch to satellite imagery, and request selections.

Built and maintained by **C-HAWQ — the Coastal Habitat and Water Quality Initiative**.

## Live site

Once GitHub Pages is enabled (Settings → Pages → Deploy from a branch → `main` / root), the dashboard is live at:

`https://<account>.github.io/<repo>/`

## What's in this repo

- **index.html** — the dashboard.
- **ResCanals_Typology_for_GitHub_10072026.zip** — required shapefile archive. Add it beside `index.html` and include it in the GitHub Pages deployment.

## Using it

Open the live link in any modern browser. An internet connection is required — the map libraries, fonts, basemap tiles, and the C-HAWQ logo load from the web. The page explains its own controls: filter with the dropdowns or by clicking a chart bar, click a canal for details and to add it to an export set, recolor from the legend, and download from the Export menu.

To preview locally, serve the folder over HTTP (`python -m http.server`) and open `index.html` — double-clicking the file won't work, because browsers block local file reads.

## Data

Each polygon is one mapped residential canal system. The dashboard reads polygon geometry and attributes directly from the required shapefile ZIP; form (`TYP_FORM`), receiving waters (`TYP_RECWATER`), and connectivity (`TYP_CONNEC`) are available as filters and map color dimensions. All remaining source attributes appear in each feature popup.

## License

Code © 2026 C-HAWQ. All rights reserved. The dashboard data is released under Creative Commons Attribution–NonCommercial–NoDerivatives 4.0 (CC BY-NC-ND 4.0). See [LICENSE](LICENSE) for details and for the terms covering the underlying public data.

## Contact

Nathan — nathan@chawq.org
