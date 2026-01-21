# Alpha Site Pipeline

AI-Powered Site Viability Scoring System for rapid school campus evaluation.

## Live Demo

**[View Dashboard](https://jjhoffstein.github.io/alpha-site-scorer/)**

## Features

### Site Scoring
- **Weighted viability scoring** — sqft, driveway, outdoor space, kitchen, zoning, cost efficiency
- **Green/Yellow/Red tiers** — 75+ Green, 50-74 Yellow, <50 Red
- **Top Pick badge** — pulsing indicator on #1 ranked site
- **Hover score breakdown** — see detailed scoring on card hover

### Pipeline Management
- **Pipeline funnel** — visual counts at each stage (Sourced → Site Visit → LOI → Negotiation → Signed)
- **Status tracking** — color-coded badges per site
- **Days in pipeline** — automatic tracking since site added
- **Stale deal alerts** — pulsing orange warning on stuck deals

### Cost Analysis
- **Break-even calculator** — factors in rent, guides, utilities, insurance, marketing, food
- **Interactive cost breakdown** — Chart.js donut visualization
- **Margin projections** — potential profit at capacity
- **Detailed explanations** — context for each cost category

### Map View
- **Interactive map** — Leaflet.js with color-coded markers
- **Auto-fit bounds** — zooms to show all sites
- **Rich popups** — score, break-even, edit/cost buttons
- **Legend** — color key overlay

### User Experience
- **Add/Edit/Delete sites** — full CRUD with live updates
- **Notes field** — broker contact, next steps, blockers
- **Click-to-edit notes** — direct access from card
- **Dark mode** — toggle with localStorage persistence
- **Mobile responsive** — works on all screen sizes
- **Keyboard shortcuts** — Cmd/Ctrl+Enter to save

### Data
- **localStorage persistence** — changes saved locally
- **CSV import** — bulk add sites via Python
- **Real demographics** — US Census API integration

## Scoring Criteria

| Factor | Weight | Description |
|--------|--------|-------------|
| Square Footage | 25 | Target student capacity (50 sqft/student) |
| Driveway Access | 15 | Controlled arrival/dismissal logistics |
| Outdoor Space | 12 | Play area, basketball, turf |
| Kitchen Area | 12 | Food service infrastructure |
| Zoning | 8 | Clear permitting path |
| Cost Efficiency | 8 | $/sqft ratio optimization |

## Stale Deal Thresholds

| Status | Days to Stale |
|--------|---------------|
| Sourced | 7 days |
| Site Visit | 14 days |
| LOI | 21 days |
| Negotiation | 30 days |

## Built With

- Python + fastcore (scoring engine)
- Vanilla JavaScript (client-side rendering)
- Chart.js (cost visualization)
- Leaflet.js (map)
- GitHub Pages (hosting)
