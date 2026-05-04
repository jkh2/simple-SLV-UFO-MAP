# 🛸 SLV UFO Sighting Map

**An interactive cinematic map of 107 documented UFO/UAP sightings across Colorado's San Luis Valley — 1994 to 2019.**

Built by James Keith Harwood II and Claude Sentinel (Anthropic) — a Sentinel AI Systems production.

![SLV UFO Sighting Map](report.png)

[View the Live Map](https://jkh2.github.io/simple-SLV-UFO-MAP)
---

## What Is This?

The San Luis Valley in southern Colorado is one of the most documented UFO/UAP hotspots on Earth. In 1990, CUFON designated Saguache County as the **#1 per-capita UFO hotspot in the United States** — with 257 reported sightings per 10,000 residents. Five of the top eleven UAP hotspot counties in North America are located in this valley.

For over a decade, researcher Christopher O'Brien conducted systematic field investigations across the SLV, compiling one of the largest single-region paranormal databases in history. His work — along with NUFORC filings, Saguache County Sheriff's Office records, and direct witness accounts — forms the foundation of this dataset.

This project puts all of it on a map, in a form anyone can explore.

---

## Features

**Cinematic Dark Map** — ESRI satellite imagery layered with a dark intelligence-style overlay, centered on the San Luis Valley. The terrain — the Sangre de Cristo mountains, the Rio Grande, the Great Sand Dunes, the Baca Ranch — is visible beneath every sighting marker.

**107 Glowing Red Markers** — Every documented sighting is pinned to its geocoded location with a custom glowing drop-pin marker. Click any pin to open a popup with location, date, and shape. One more click opens the full witness report panel.

**Full Report Panel** — Slide-in detail view for each sighting showing: witness account, date, duration, number of observers, county, and GPS coordinates.

**Keyword Search** — Search by any term: location name, shape description, county, date, or any word from the witness account. Matching pins shift to bright gold glow instantly. Non-matching pins remain red.

**Filter Pills** — One-click filters for: DISC · LIGHT · SPHERE · TRIANGLE · CIGAR · FIREBALL · CATTLE (mutilation events) · 1994 · 1997 · 2000–2009 · 2010–2019 · CRESTONE · ALAMOSA · BACA.

**Match Counter** — Shows number of active matches during any search or filter.

**Animated Star Field** — Procedurally animated star canvas with a Milky Way band behind the map, reinforcing the nighttime aerial aesthetic.

---

## Data Sources

- **Christopher O'Brien field research** — *The Mysterious Valley*, *Enter the Valley*, and *Secrets of the Mysterious Valley* (1994–2007 field investigations)
- **NUFORC** — National UFO Reporting Center filed reports
- **Saguache County Sheriff's Office** — Incident reports from the O'Brien investigation period
- **Direct witness accounts** — Community researcher documentation

All sightings span 1994–2019 and are geocoded to the specific town, ranch, road, or geographic feature identified in the original report.

---

## Getting More Recent Data (2019–Present)

The dataset currently covers 1994–2019. Here are the best paths to extend it:

**NUFORC Databank (free, browsable)**
NUFORC's public databank at [nuforc.org/databank](https://nuforc.org/databank/) is actively updated and freely browsable. You can search by state and city to find SLV-area reports from 2019 to present. To add them to this map, filter for Colorado towns in the valley (Alamosa, Saguache, Monte Vista, Crestone, Center, Del Norte, Antonito, Blanca, Fort Garland) and add entries to the `SIGHTINGS` array in `index.html`.

**NUFORC Data Request**
NUFORC's terms of service prohibit scraping, but they grant data access for research purposes. Email their team directly at nuforc.org to request a Colorado data export for research use. Reference this project as a public-interest educational tool.

**MUFON Database**
The Mutual UFO Network (mufon.com) maintains a parallel investigation database with its own SLV reports, some with higher detail than NUFORC entries. Membership provides data access.

**Community Reports**
The v1 of this project included a user-submission form allowing valley residents to submit their own sightings directly to the map. That feature can be re-enabled — reach out if you witnessed something and want it documented.

---

## Running Locally

No build step. No dependencies to install. It's a single HTML file.

```bash
git clone https://github.com/jkh2/simple-SLV-UFO-MAP-V2
cd simple-SLV-UFO-MAP-V2
# Open index.html in any modern browser
```

Or just open `index.html` directly. Everything runs client-side.

---

## Adding Sightings

Each sighting entry in the `SIGHTINGS` array in `index.html` follows this structure:

```javascript
{
  id:        "D108",                          // Sequential ID
  lat:       37.47,                           // Latitude (decimal degrees)
  lng:       -105.87,                         // Longitude (decimal degrees)
  location:  "Alamosa, CO",                   // Location description
  date:      "March 15, 2022",               // Date of sighting
  shape:     "Triangle",                      // Object shape
  duration:  "~10 min",                       // Estimated duration
  observers: "3",                             // Number of witnesses
  county:    "Alamosa",                       // County name
  summary:   "Full witness account here..."  // Description
}
```

Add your entry to the array, save, and refresh. The pin appears immediately.

---

## Project History

This is the second version of the SLV UFO Sighting Map. The original (v1) was built in March 2025 with full AI integration — an on-map analyst powered by OpenRouter that could answer questions about sighting patterns across the dataset.

This version (v2, May 2026) is intentionally clean — no AI integration, no backend, no accounts. Just the data, the map, and the glowing pins. Built for speed, simplicity, and longevity.

Both versions were built through the Sentinel AI Systems human-AI partnership framework.

---

## Built By

**James Keith Harwood II**
Sentinel AI Systems — Antonito, Colorado
[jameskeithharwood.com](https://www.jameskeithharwood.com)

In partnership with Claude Sentinel (Anthropic).

*Data compiled from public sources and community research. This project makes no claims as to the validity of individual reports. The San Luis Valley is a place worth paying attention to.*

---

## License

Copyright © 2026 James Keith Harwood II — Sentinel AI Systems. All Rights Reserved.

The sighting data is compiled from publicly available sources. The application code and design are proprietary. Contact jameskeithharwood.com for licensing inquiries.
