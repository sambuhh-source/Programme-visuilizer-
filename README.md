# SDC Builders — Programme Visualiser

An interactive, single-file Gantt chart and construction programme visualiser built for SDC Builders Ltd's Stirling Building Refurbishment (Project EM01488, University of Cambridge).

**[Open the live app](./index.html)** — download `index.html` and open it in any modern browser. No install, no server, no build step.

## What it does

- Interactive Gantt chart with day/week/month/quarter views, zoom, and a minimap
- Drag-to-reschedule tasks with automatic dependency cascading (FS/SS/FF/SF), undo/redo
- Critical path highlighting, milestones, progress tracking, baseline comparison
- Filtering by trade, floor, date range, and critical-path-only, with fade-not-hide behaviour
- **Floor View**: visualise programme tasks directly on 12 real General Arrangement drawings from the project (main building levels B1–06, plus all five North Pavilion sheets), with click-to-place room markers
- Asta Powerproject PDF import with a best-effort parser and editable preview before committing
- Everything saved to your browser's local storage; export/import as JSON for backup or sharing

Pre-loaded with the real 801-task Best Build Programme (Rev A) across 20 work-package zones.

## Usage

1. Download `index.html`
2. Open it directly in Chrome, Edge, or Firefox — that's it

All data stays in your browser. Nothing is sent anywhere.

## Resetting sample data

If you've previously opened an older version of this file, your browser may have saved that version's data locally, which will take precedence on reload. Click the reset icon in the header (next to Help) to clear it and reload the built-in sample data.

## Tech

Single HTML file, vanilla JS, no build step. Uses PDF.js (via CDN) for PDF import parsing. GA drawings are rasterised and embedded directly in the file for fully offline use after first load.
