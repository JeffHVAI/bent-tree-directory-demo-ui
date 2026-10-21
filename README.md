# Bent Tree Directory Demo UI

Interactive commercial building directory and wayfinding demo UI designed for Hoververse SurfaceWare touchless displays.

## Live Demo
- **GitHub Pages**: [https://jeffhvai.github.io/bent-tree-directory-demo-ui/](https://jeffhvai.github.io/bent-tree-directory-demo-ui/)

## Overview
- **Display Creator Spec**: `Bent Tree Directory.dc.html` / `index.html`
- **Canvas**: 1920x1080 display configuration with dynamic split zones (left media/announcements, right directory & wayfinding)
- **Components & Scripts**:
  - `image-slot.js` — Custom web component for image rendering and placeholders
  - `support.js` — Data models, reactive bindings, and directory interactions
- **SurfaceWare Touchless Ergonomics & Gestures**:
  - **Anti-Gorilla Arm Architecture**: Eye-level upper region reserved for passive viewing (informational headers, media carousel, 3D map); all actionable controls (tabs, directory cards, "Show me the way" primary CTA, floor selectors) centered in the natural chest/heart mid-section directly in front of the standing user (right interaction zone) to prevent shoulder elevation fatigue.
  - **Anti-Parallax Centering**: Actionable controls kept centered at heart height and safely away from display edges or the extreme bottom floor/waist boundaries where optical sensor ray angles and parallax distortion peak.
  - **Point-to-Click Dwell Engine**: Pointing and resting on any actionable card or button activates a glowing 60fps countdown reticle; after a calibrated ~950ms dwell, it automatically triggers a click with haptic/visual scale pop. Physical click and tap remain supported immediately.
  - **Inverted Gesture Scrolling**:
    - **Wave UP** (`dy < 0` / `ArrowDown`): Scrolls content upward to reveal items below the line.
    - **Wave DOWN** (`dy > 0` / `ArrowUp`): Scrolls content downward to return to top.
    - **Wave Sideways** (`dx` / `ArrowLeft`/`ArrowRight`): Switches category tabs or navigates back.
  - **Direct Ad Engagement**: Lower actionable CTA buttons on media slides allow instant navigation into tenant wayfinding profiles directly from featured campaigns.
- **Featured Tenants & Campaigns**:
  - **LifeGenix Institute (Anchor Tenant, Suite 100)**: Dallas's premier early detection center featuring full-body MRI & CT scans, non-surgical spine treatments, and cellular regenerative medicine
  - **TrustUp (Suite 120)**: Elite "Ring of Life" training center integrating asset protection and wealth building with metabolic health and peak fitness
  - **Hover OS (Suite 250)**: Headless operating system for touchless user experiences
  - **Hover Health**: Sterile touchless clinical workflows for healthcare, ORs, and cleanrooms
  - **Hover Aero**: Touchless passenger self-service, check-in, and flight information display systems
  - **Hover Engage**: Living Heritage projection-mapped interpretive exhibits that disappear when idle
  - **Hover Guide**: Adaptive 3D stacked multi-floor wayfinding and real-time Blue Dot maps
  - **Tenant & Building Announcements**: Parkline Dental, Helix BioSystems, Wells Ridge Wealth Advisors, Building Notices

## Repository Layout
```
├── index.html                    # Root web entrypoint for GitHub Pages
├── Bent Tree Directory.dc.html   # Main Display Creator layout & styles
├── image-slot.js                 # Custom <image-slot> element definition
├── support.js                    # Logic and runtime support
├── assets/
│   ├── HoverVerse_Logomark_*.svg # Brand SVGs
│   └── ads/                      # Slide media (Hover OS, Health, Aero, Engage, Guide, etc.)
└── uploads/
    └── 17230 Bent Tree 1st Layout (1).pdf # Floor layout plans
```
