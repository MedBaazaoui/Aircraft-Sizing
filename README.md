# The Drafting Table — Aircraft Preliminary Sizing Tool

A browser-based preliminary sizing wizard for fixed-wing aircraft, covering the full conceptual design sequence from category selection through power plant estimation.

**Live tool → [medbaazaoui.github.io/Aircraft-Sizing](https://medbaazaoui.github.io/Aircraft-Sizing/)**

---

## What it does

Works through 9 sequential steps that mirror the conceptual design process taught in aerospace engineering programs and used in early-stage aircraft development:

1. **Aircraft category** — FAR Part 103 ultralight, LSA, GA single/twin, regional turboprop, jet transport
2. **Mission & weights** — payload, range, fuel fraction estimation via Breguet-derived methods
3. **Wing geometry** — aspect ratio, taper, sweep, area, span, and stall speed
4. **Fuselage sizing** — length, fineness ratio, wetted area
5. **Tail surfaces** — horizontal and vertical tail sizing via volume coefficients
6. **Airfoil selection** — NACA 4-series library with lift curve slope and Clmax data
7. **Propulsion** — power loading, thrust-to-weight ratio, engine sizing
8. **Performance check** — cruise speed, climb rate, and range cross-verification
9. **Summary & export** — full parameter sheet, 2D three-view SVG silhouette, CSV/JSON dual-unit export

All calculations run client-side. No data is sent anywhere. No login required.

---

## Who it's for

- Aviation students working through a first conceptual design exercise
- Homebuilders and kit aircraft designers doing early feasibility checks
- Engineers wanting a quick sanity-check on weight fractions and geometry before moving to CAD
- Anyone curious about how a paper airplane turns into real numbers

---

## Technical notes

- Single HTML file, no dependencies, no build step
- Session system supports up to 6 named design snapshots with save/restore
- Silhouette engine draws a calibrated 2D three-view from computed geometry parameters
- All outputs available in both SI and imperial units

---

*Built by [Med Baazaoui](https://github.com/medbaazaoui) — freelance developer and designer.*
