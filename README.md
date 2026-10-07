# FiftyStates

A responsive, browser-local travel map of all 50 U.S. states, inspired by Unseen Bangladesh. Original FiftyStates interface and code.

## Features

- Click or keyboard-select states on a geographic map; search and browse by region.
- Saved visited states, traveler name, labels, and five color themes in localStorage.
- Download a personalized high-resolution PNG, JPG, or PDF.
- Explore state-specific official National Park Service pages.
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
- Typography: DM Sans and Playfair Display served by Google Fonts, with system fallbacks.

Alaska and Hawaii use map insets. D.C. and territories are not included in the 50-state count. Browser storage is device-local and not synchronized. Destination discovery links to NPS; a full travel-guide database, itinerary planner, games, and community submissions are future features.
