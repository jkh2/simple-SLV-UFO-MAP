# 🛸 SLV UFO Sighting Map

**An interactive cinematic map of 107 documented UFO/UAP sightings across Colorado's San Luis Valley — 1994 to 2019.**

Built by James Keith Harwood II and Claude Sentinel (Anthropic) — a Sentinel AI Systems production.

![SLV UFO Sighting Map](report.png)

[View the Live Map](https://jkh2.github.io/simple-SLV-UFO-MAP/index.html)

---

## What Is This?

The San Luis Valley in southern Colorado is one of the most documented UFO/UAP hotspots on Earth. In 1990, CUFON designated Saguache County as the **#1 per-capita UFO hotspot in the United States** — with 257 reported sightings per 10,000 residents. Five of the top eleven UAP hotspot counties in North America are located in this valley.

For over a decade, researcher Christopher O'Brien conducted systematic field investigations across the SLV, compiling one of the largest single-region paranormal databases in history. His work — along with NUFORC filings, Saguache County Sheriff's Office records, and direct witness accounts — forms the foundation of this dataset.

This project puts all of it on a map, in a form anyone can explore.

---

## Features

**Cinematic Dark Map** — ESRI satellite imagery layered with a dark intelligence-style overlay, centered on the San Luis Valley. The terrain — the Sangre de Cristo mountains, the Rio Grande, the Great Sand Dunes, the Baca Ranch — is visible beneath every sighting marker. An animated star field with a Milky Way band reinforces the nighttime atmosphere.

**107 Glowing Red Markers** — Every documented sighting is pinned to its geocoded location with a custom glowing drop-pin SVG marker. Hover any pin and it displays READ REPORT.

**🛸 UFO Reveal Animation** — Click any pin and a flying saucer screams in from a random screen edge, arcs toward that location, descends, and deploys a tractor beam. The full witness report slides open mid-beam as if the data is being pulled down from the craft. The UFO bobs, then cuts the beam and shoots away. Also appears as an ambient flyby every 30–60 seconds.

**Full Report Panel** — Slide-in detail view showing the complete witness account, date, duration, number of observers, county, and GPS coordinates.

**🔗 Shareable Report Links** — Every report panel includes a SHARE THIS REPORT link that copies a direct URL to your clipboard. Share any sighting on Facebook and the map opens straight to it — UFO flies directly to that pin.

**Keyword Search** — Search by any term: location, shape, county, date, or any word from the witness account. Matching pins instantly shift to bright gold glow. Search results also summon the UFO to the first result.

**Filter Pills** — One-click filters for: DISC · LIGHT · SPHERE · TRIANGLE · CIGAR · FIREBALL · CATTLE · 1994 · 1997 · 2000–2009 · 2010–2019 · CRESTONE · ALAMOSA · BACA.

**📅 Year Slider** — Single-handle slider at the bottom filters the map by year. A mini bar chart above shows sightings per year — hover any bar for the exact count, click any bar to jump to that year. ALL YEARS resets instantly.

**🔥 Heat Map** — Toggle a canvas-based density overlay that renders glowing red zones where sightings cluster. Updates live when the year filter is active.

**🛸 Random Report** — One click summons the UFO to a surprise sighting. The map pans to the location, the UFO flies in, and the report reveals.

**📊 County Breakdown** — The control panel ranks every county by sighting count with a proportional bar chart. Saguache County's dominance is immediately visible.

**Draggable Control Panel** — The controls panel (Random Report, Heat Map, legend, county chart) is fully draggable. Grab the CONTROLS grip bar and move it anywhere. Touch-enabled for mobile.

---

## Data Sources

- **Christopher O'Brien field research** — *The Mysterious Valley*, *Enter the Valley*, and *Secrets of the Mysterious Valley* (1994–2007 field investigations)
- **NUFORC** — National UFO Reporting Center filed reports
- **Saguache County Sheriff's Office** — Incident reports from the O'Brien investigation period
- **Direct witness accounts** — Community researcher documentation

All sightings span 1994–2019 and are geocoded to the specific town, ranch, road, or geographic feature identified in the original report.

---

## Getting More Recent Data (2019–Present)

**NUFORC Databank (free, browsable)**
NUFORC's public databank at [nuforc.org/databank](https://nuforc.org/databank/) is actively updated. Search by state and city for SLV towns: Alamosa, Saguache, Monte Vista, Crestone, Center, Del Norte, Antonito, Blanca, Fort Garland. Add findings to the `SIGHTINGS` array in `index.html`.

**NUFORC Data Request**
NUFORC prohibits scraping but grants research access. Email them at nuforc.org referencing this project as a public-interest educational tool.

**MUFON Database**
The Mutual UFO Network (mufon.com) maintains a parallel database with its own SLV reports. Membership provides data access.

---

## Running Locally

No build step. No dependencies. Single HTML file.

```bash
git clone https://github.com/jkh2/simple-SLV-UFO-MAP
cd simple-SLV-UFO-MAP
# Open index.html in any modern browser
```

---

## Adding Sightings

Each entry in the `SIGHTINGS` array in `index.html`:

```javascript
{
  id:        "D108",
  lat:       37.47,
  lng:       -105.87,
  location:  "Alamosa, CO",
  date:      "March 15, 2022",
  shape:     "Triangle",
  duration:  "~10 min",
  observers: "3",
  county:    "Alamosa",
  summary:   "Full witness account here..."
}
```

Add the entry, save, refresh. The pin appears immediately with full UFO interaction.

---

## Community

This map is offered as a resource to the San Luis Valley community — especially the members of **[Everything SLV](https://www.facebook.com/groups/645890198862657)** on Facebook, whose group has kept the spirit and stories of the valley alive. A small tribute in the corner of the map is the least we could do.

---

## Project History

This is the second version of the SLV UFO Sighting Map. The original (v1, March 2025) featured full AI integration — an on-map analyst powered by OpenRouter. This version (v2, May 2026) is intentionally clean — no AI, no backend, no accounts. Just the data, the map, the glowing pins, and a flying saucer that delivers the reports.

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
