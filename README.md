# The Drafting Table

Free, browser-based tools for preliminary aircraft design. No sign-up, no install, no paywall.

**Live site → [medbaazaoui.github.io/Aircraft-Sizing](https://medbaazaoui.github.io/Aircraft-Sizing/)**

The Drafting Table is for the first design pass: deciding what the aircraft should be before moving to CAD, OpenVSP, XFLR5 or a full structural analysis. It replaces the unchecked spreadsheets and hand calculations that this stage usually relies on.

---

## Tools

### 1. Aircraft Sizing

A nine-step guided wizard from category to a full parameter sheet, with a live drawing that updates as you change inputs.

1. **Category & configuration**: FAR Part 103 ultralight, light-sport (LSA), experimental, STOL and other categories set the defaults
2. **Weight estimation**: gross weight, payload and fuel
3. **Wing loading & stall speed**: the core trade-off between stall speed, wing loading and CLmax
4. **Wing area, span & chord**: from wing loading and aspect ratio
5. **Airfoil selection & angles**: airfoil library filtered by Reynolds number and required CLmax, with finite-wing correction
6. **Fuselage & tail arm**
7. **Tail sizing**: volume coefficients
8. **Power & propeller**: power loading, engine choice and a cruise performance check
9. **Design summary & export**: full parameter sheet compared against a verified reference-aircraft database, three-view silhouette, CSV and JSON export

Also: up to six design tabs side by side, metric and imperial units, and a print layout.

### 2. Structural V-n

Structural checks for a preliminary wing design, fed by the Aircraft Sizing results.

- V-n (flight envelope) diagram
- Main and rear spar bending and shear checks
- **Torsion check** for stressed-skin and fabric/truss construction, including the combined bending, shear and torsion check at each spar web
- Cable and turnbuckle strength data for wire-braced designs, taken from manufacturer specifications
- **Compare Scenarios** to put two design options side by side
- CSV, JSON and print export

---

## Who it is for

- Aviation and aerospace students on a first conceptual design exercise
- Homebuilders and kit-aircraft designers doing early feasibility checks
- Engineers who want a quick sanity check before moving to heavier tools

---

## Accuracy and limits

These tools are for **preliminary design and education only**. They are not a substitute for a qualified engineer, a certification process, or testing.

- Formulas come from standard references (for example Raymer, Roskam, Gudmundsson, Megson). Reference-aircraft data and hardware strengths are checked against primary sources, and data that cannot be verified is not included.
- Each tool states what it does not model. Read those notes before relying on a result.
- Found a wrong number? Please open an issue with the inputs you used and the source you think is right.

---

## Running it yourself

Each tool is a single self-contained HTML file with no dependencies and no build step.

```
index.html            landing page
Aircraft-Sizing.html  tool 1
Structural-VN.html    tool 2
```

Clone the repository and open any file in a browser. It also works offline once loaded.

---

## Contributing

Bug reports, wrong-data reports, and feature requests are welcome through GitHub issues. If you have a source for open, reusable data (airfoil coordinates, reference aircraft, hardware strengths), please link it in the issue.

## Support

The tools are free and will stay free. If they are useful to you, you can support the project on [Patreon](https://www.patreon.com/cw/TheDraftingTable). Sending feedback or suggesting features never requires paying.

---

*Built by [Med Baazaoui](https://github.com/medbaazaoui), freelance developer and engineer.*
