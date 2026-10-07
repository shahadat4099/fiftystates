# FiftyStates

A personal atlas of all 50 U.S. states with an original map-first layout, accessible state editor drawer, customization panel, and editorial destination cards.

## Features

- Native dialog panels for state editing and map customization, with Escape and focus restoration.
- Click or keyboard-select states on a geographic map; search and browse by region.
- Saved visited states, traveler name, labels, and five color themes in localStorage.
- Download a personalized high-resolution PNG, JPG, or PDF.
- Explore state-specific official National Park Service pages and three featured parks.
- Public-domain photos: Acadia by NPS/Victoria Stauffenberg (https://npgallery.nps.gov/AssetDetail/1cde9bcf-cc98-4513-8e06-fcf608af25ab), Great Sand Dunes by NPS/Mackenzie Reed (https://npgallery.nps.gov/AssetDetail/bfad0ff7-10ce-458a-b02d-56b8cfee10a8).
- Responsive desktop/mobile layout; no account, backend, or analytics.

## Run locally

From the repository directory:

```sh
python3 -m http.server 8000
```

Open http://localhost:8000. A server is needed for the local map JSON; opening index.html directly is unsupported.

## Publish

In GitHub repository Settings → Pages, select Deploy from a branch, main, / (root). All paths are relative, so this works on GitHub project pages. No build step is needed.

## Data and credits

- Geometry: US Atlas 3.0.1, derived from the U.S. Census Bureau. https://github.com/topojson/us-atlas
- D3 7.9.0 (ISC); TopoJSON Client 3.1.0 (ISC); jsPDF 2.5.2 (MIT). Vendored with upstream license notices; full licenses in vendor/.
- Grand Teton photograph: NPS staff, public domain, from Wikimedia Commons: https://commons.wikimedia.org/wiki/File:Views_at_Grand_Teton_National_Park,_Wyoming_(f07dce63-49b2-4c89-b600-0f9f28b92570).jpg
- Typography: self-hosted Inter and Manrope, licensed under SIL OFL (license files in assets/fonts/), with system fallbacks.

Alaska and Hawaii use map insets. D.C. and territories are not included in the 50-state count. Browser storage is device-local and not synchronized. Destination discovery links to NPS; a full travel-guide database, itinerary planner, games, and community submissions are future features.
