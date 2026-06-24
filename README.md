# DataCore — Data Collection Center Website

A modern, responsive marketing website for a data collection center platform. Built with vanilla HTML, CSS, and JavaScript — no frameworks or build tools required.

## Overview

DataCore presents an enterprise data collection platform with a dark, tech-forward aesthetic. The site communicates the platform's core value proposition: aggregating, processing, and delivering data from any source at scale.

## Pages & Sections

| Section | Description |
|---|---|
| **Hero** | Animated node-graph canvas, headline, and CTA buttons |
| **Metrics Bar** | Key stats: 12 TB/day, 99.98% uptime, <40ms latency, 200+ connectors |
| **Features** | Six capability cards — ingestion, connectors, governance, schema, transforms, observability |
| **Pipeline** | Five-step flow: Collect → Validate → Transform → Store → Deliver |
| **Sources** | Six data source types with Live / Batch / Stream badges |
| **CTA** | Trial and sales conversion section |
| **Footer** | Branding and copyright |

## File Structure

```
/
├── index.html   # All HTML, CSS, and JS in one self-contained file
└── README.md    # This file
```

## Features

- **Mobile responsive** — adapts across desktop (1100px+), tablet (640–900px), and mobile (<640px)
- **Animated hero canvas** — live WebGL-style node graph with traveling data packets (Canvas 2D API)
- **Mobile navigation** — hamburger menu with overlay for small screens
- **Reduced motion support** — respects `prefers-reduced-motion` OS setting
- **No dependencies** — only Google Fonts (Space Grotesk + Inter) loaded via CDN
- **Accessible** — semantic HTML5, ARIA labels on interactive elements, keyboard-navigable

## Design Tokens

| Token | Value | Usage |
|---|---|---|
| `--navy` | `#0A0F1E` | Page background |
| `--cyan` | `#00D4FF` | Primary accent, CTAs |
| `--steel` | `#8899AA` | Body text, descriptions |
| `--light` | `#E8EEF4` | Headings, primary text |
| `--card` | `#111827` | Card and section backgrounds |
| `--green` | `#00E5A0` | Live status, data packets |
| `--purple` | `#7C6EF8` | Batch badge accent |

## Typography

- **Display / Headings:** Space Grotesk (700, 600)
- **Body / UI:** Inter (400, 500)

## Running Locally

No build step needed. Open `index.html` directly in any modern browser:

```bash
# Option 1 — open directly
open index.html

# Option 2 — serve with Python
python3 -m http.server 8080

# Option 3 — serve with Node
npx serve .
```

## Browser Support

Works in all modern browsers (Chrome, Firefox, Safari, Edge). Canvas animation degrades gracefully in environments that disable JavaScript.

## Customization

To update branding, edit the CSS variables in `:root` at the top of the `<style>` block. To change copy, update the text content in the HTML. No compilation needed.

---

© 2026 DataCore Inc.
