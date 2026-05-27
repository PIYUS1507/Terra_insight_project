# PortPulse — Weekly Demand Grid

An interactive planning dashboard built as a single self-contained HTML file. No build step, no dependencies, no server required.

## Running the App

Double-click `index.html` to open it in your browser.

That's it.

---

## Features

### Core Grid
- Renders all items with columns: Item, Category, Region, Status, W1–W8, Total
- Colour-coded demand cells per item target — **green** (≥ 90%), **amber** (50–89%), **red** (< 50% or zero)
- Status badges styled for `active`, `paused`, and `discontinued`
- Summary row at the bottom showing column totals — updates dynamically with filters

### Filtering & Sorting
- **Category dropdown** — filter to a single category or show all
- **Status chips** — toggle active, paused, and discontinued items independently
- **Column sorting** — click any W1–W8 header to sort ascending → descending → off, with ▲/▼ indicator
- **Reset button** — clears all filters and sorting in one click

### Detail Panel
- Click any row to open a slide-in panel showing:
  - Average weekly demand, target, total demand, zero-week count
  - Overall tracking status (On Target / Below Target / At Risk)
  - Sparkline bar chart of weekly trend
  - Week-by-week breakdown with colour-coded progress bars
- Clicking another row updates the panel without closing it
- Close with the ✕ button or `Escape`

### Add New Item
- Click **Add Item** to open a modal form
- Fields: Item name, Category, Region, Target, Status, W1–W8 demand values
- Inline validation — no browser `alert()` dialogs
- New item appears in the grid immediately, fully filterable and sortable

### Bonus
- Items persist across page refreshes via `localStorage`
- Keyboard accessible: `Escape` closes modal or panel

---

## Tech Stack

Plain HTML, CSS, and JavaScript — no frameworks, no build tools, no external files except Google Fonts (loaded over CDN). The file works offline if fonts fall back to system sans-serif.

---

## Project Structure

```
index.html   ← entire application (HTML + CSS + JS inline)
README.md
```

---

*Terra Insight Pvt. Ltd. · PortPulse Intern Evaluation Test · May 2026*
