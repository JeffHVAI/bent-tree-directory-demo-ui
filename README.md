# Bent Tree Directory Demo UI

Interactive commercial building directory and wayfinding demo UI designed for Hoververse SurfaceWare touchless displays.

## Overview
- **Display Creator Spec**: `Bent Tree Directory.dc.html`
- **Canvas**: 1920x1080 display configuration with dynamic split zones (left media/announcements, right directory & wayfinding)
- **Components & Scripts**:
  - `image-slot.js` — Custom web component for image rendering and placeholders
  - `support.js` — Data models, reactive bindings, and directory interactions
- **Assets**: Tenant advertisements, PSA slides, floor plan layouts, and brand logomarks

## Repository Layout
```
├── Bent Tree Directory.dc.html   # Main Display Creator layout & styles
├── image-slot.js                 # Custom <image-slot> element definition
├── support.js                    # Logic and runtime support
├── assets/
│   ├── HoverVerse_Logomark_*.svg # Brand SVGs
│   └── ads/                      # Slide media (fire, helix, parking, parkline, wells)
└── uploads/
    └── 17230 Bent Tree 1st Layout (1).pdf # Floor layout plans
```
