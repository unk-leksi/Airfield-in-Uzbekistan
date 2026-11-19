# 🗺️ Interactive Airfield Map (Uzbekistan) with Navigation Waypoints and No-Fly Zones

A web page displaying the air navigation environment around an airfield in Uzbekistan. Built with Leaflet and open map data.

## ✨ What the Map Shows

*   **Navigation waypoints** — marked with blue triangles and labels (MIKNO, ODORI, DOSOR, BAMUT, TULGA, IBMOB, DIBAD, DILRO, TISIB, KUFIM, MUVIT, OGRIP, ROSEG, GESOR, BASUG, GUSAR, OSBOR, MOVUP, ULKUB, OSDAK, MUSON, and others).
*   **Special oval-marked points** — KUFIM, DD004, DD002, TL303 (highlighted with oval outlines).
*   **Airfield Reference Point (KTA)** — marked with a red "КТА" label near the runways.
*   **Runways** — two runways (08L/26R and 08R/26L) drawn as black lines with width-based thickness.
*   **Routes and lines** — connect waypoints; line color and style vary (black, green dashed, orange).
*   **No-fly zones** — 6 zones (UT(P)101 – UT(P)106) shown as red circles with popups.
*   **Orange border** — a polyline marking a specific boundary (with an "Orange border" popup).
*   **Altitudes** — text labels (7000ft, 8000ft, FL150, etc.) at their respective coordinates.

## 🛠️ Tech Stack

*   **HTML5 / CSS3** — structure and styling.
*   **JavaScript** — rendering logic for all map objects.
*   **Leaflet** (via CDN `unpkg.com`) — interactive map engine.
*   **SVG / DivIcon** — for triangle markers, oval outlines, and text labels.
*   **GitHub Pages** — hosting for the static page.

## 🚀 Run Locally

1.  Clone the repository:
    ```bash
    git clone https://github.com/YOUR_USERNAME/YOUR_REPO.git
