# 🗺️ Interactive Airfield Maps (Uzbekistan) — Waypoints, Runways & No-Fly Zones

A set of two interactive web maps displaying the air navigation environment around an airfield in Uzbekistan. Built with Leaflet and open map data. Each map shows a different set of waypoints, routes, altitudes and special zones.

## 📂 Project Structure

| File | Description |
|------|-------------|
| `map.html`  | First version of the airfield map (waypoints, routes, runways, no-fly zones, altitudes). |
| `map2.html` | Extended version with an additional set of waypoints (ZT, UT, AT series), new routes, and extra oval-marked points. |
| `README.md` | This documentation. |

Both pages are standalone HTML files — no build step required.

## ✨ What the Maps Show

### Common features (both maps)
*   **Airfield Reference Point (KTA)** — marked with a red "КТА" label near the runways.
*   **Runways** — two runways (**08L/26R** and **08R/26L**) drawn as black lines with width-based thickness.
*   **No-fly zones** — 6 zones (**UT(P)101 – UT(P)106**) shown as red circles with popups.
*   **Orange border** — a long polyline marking a specific boundary (popup "Orange border").
*   **Altitudes** — text labels (e.g. 7000ft, 8000ft, 13000ft, FL150, FL200) at their coordinates.
*   **Base layers** — Esri National Geographic (primary) + Esri World Hillshade (semi-transparent relief, opacity 0.35).
*   **Coordinate system** — WGS84 (decimal degrees), map centered at `[41.41, 69.28]`, zoom 8.

### `map.html` — first version
*   **Waypoints** (blue triangles + labels): MIKNO, ODORI, DOSOR, BAMUT, TULGA, IBMOB, DIBAD, DILRO, TISIB, KUFIM, MUVIT, OGRIP, ROSEQ, GESOR, BASUG, GUSAR, OSBOR, MOVUP, ULKUB, OSDAK, MUSON, plus AS/AR/TL/DD series points.
*   **Routes** — black lines, green dashed lines, and orange route segments.
*   **Special oval-marked points** — KUFIM, DD004, DD002, TL303.

### `map2.html` — extended version
*   **Additional waypoints**: ZT101–ZT109, UT201–UT204, AT234–AT238, ABMEM, DD087, GIVOM, ZEVIT, NOVAB, AD010, KARIZ, ZARKU, LIPOV, SANUP, REGSO, PIVIN, NIPVI, DD001–DD004, and others.
*   **New routes** connecting the added points (ZT/UT/AT chains, DD routes, green KTA routes, etc.).
*   **Special oval-marked points** — AT234, KUFIM, ZT102, DD003.
*   **Includes `leaflet.polylineDecorator`** (loaded via CDN) — ready for dashed/arrow route styling.
*   **Altitudes** include additional values such as 1200ft, 3300ft, 4000ft, 5000ft, FL150, FL200.

## 🛠️ Tech Stack

*   **HTML5 / CSS3** — structure and styling.
*   **JavaScript** — rendering logic for all map objects.
*   **Leaflet** (via CDN `unpkg.com`) — interactive map engine.
*   **Leaflet PolylineDecorator** (CDN `cdnjs.cloudflare.com`, used in `map2.html`) — for decorated route lines.
*   **SVG / DivIcon** — for triangle markers, oval outlines, and text labels.
*   **GitHub Pages** — hosting for the static pages.

## 🚀 Run Locally

1.  Clone the repository:
    ```bash
    git clone https://github.com/YOUR_USERNAME/YOUR_REPO.git
