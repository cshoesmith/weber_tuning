# Weber Carburetor Jetting Calculator v3

A standalone Weber carburetor jetting calculator built around baseline Weber formulas plus conservative tuning heuristics for DCOE, IDF, and 32/36 progressive setups.

## Features

- **61 Engine Database**: Toyota, Honda, Mazda, Nissan/Datsun, Alfa Romeo (1960-2010)
- **Multiple Weber Families**: DCOE sidedraft, IDF downdraft, and 32/36 progressive baselines
- **Setup Selector**: DCOE single/twin/triple, IDF single/twin, and 32/36 progressive single
- **Physical Setup Limits**: Carburetor layouts are now restricted so total venturi count cannot exceed the engine's cylinder/rotor count
- **Stronger Cam Modeling**: Stock, street, and race cams now shift venturi suggestions plus main, idle, pump, and air-corrector baselines more noticeably
- **Engine Summary Header**: The Recommended Baseline panel now shows the selected engine or custom setup summary, including displacement, cylinder/rotor count, RPM, and cam profile
- **Setup Preview**: Recommendations now begin with the selected carb setup, a visual illustration, and per-venturi/per-barrel load context
- **Configuration Health Score**: Enforce the choke/jet sizes you actually have, then see whether the remaining circuits can compensate or whether the combo is a poor fit
- **Override Reset Buttons**: Each available-parts override field now has its own Reset button to return that selector to Auto / baseline instantly
- **Body-Specific Choke Availability**: DCOE and IDF venturi choices now change with carb body size so unrealistic pairings are filtered out up front
- **Baseline Weber Formulas**: Family-specific main and air correction rules, plus idle/emulsion/needle starting points
- **Supports**: 4-cyl, 6-cyl, and rotary engines (985cc - 3500cc)
- **Configurations**: DCOE single/twin/triple, IDF single/twin, and 32/36 progressive single
- **Auto-venturi**: Suggests appropriate choke size based on displacement and approximate stock peak-power RPM
- **About Button**: Shows project contact details, MIT license information, and a donation placeholder button
- **Reference Tables Button**: Opens all lookup tables and advisory material directly from the main page
- **Reference Links Button**: Opens source links formatted in Chicago-style bibliography form
- **Guided 3-Step Wizard**: The app now walks users through carburetor choice, engine selection/manual entry, and finally a tuning report with live tweak controls
- **Progress & Completion Feedback**: Each stage shows where the user is in the flow and confirms when a setup step has been completed
- **Report-Style Results**: The final screen keeps the existing calculated data, health score, formulas, advisories, and AFR view in a cleaner report layout

## Usage

1. Open `index.html` or `weber_calculator.html` in any web browser
2. In step 1, choose the Weber carburetor family and count you want to tune
3. In step 2, either select a make/engine from the database to auto-fill the basics or enter your build manually
4. Continue to the report screen to review the calculated baseline, engine/setup summary, and health score
5. Tweak carb body, venturi/choke, idle air bleed or holder family, and available-parts overrides directly from the report screen as needed
6. Recommendations update live as settings change, with a brief visual highlight when the calculated results change

### Mobile Workflow Notes

- On mobile-sized screens, the calculator now behaves like a true 3-screen wizard instead of stacking the full workflow onto one page
- The default 2000cc example no longer leads the experience; users start by choosing a carburetor setup, then move into engine selection or manual entry
- Compatibility filtering for carb layouts is applied after the engine step, so the first screen stays focused on carburetor choice without premature restrictions
- The report view still contains the same calculated baseline, health score, formulas, advisories, and AFR chart data as the desktop experience, but now also hosts the tweak controls for available hardware

## Engine Coverage

### Toyota (17 engines)
2K/3K/4K, 2E, 2TC, 3TC, 2T-G, 4A-GE (16V/20V), 18R-G, 22R, 3S-GE/GTE, 5S-FE, 7M-GE, 1JZ/2JZ

### Honda (12 engines)  
EB/EJ/EW, ZC, D16, B16A/B, B18C, H22A, F20C, K20A, K24A

### Mazda (10 engines)
PC/PB/B3/B6, BP-ZE, FS-DE, FE-DOHC, KL-ZE, 13B, 20B Rotary

### Nissan/Datsun (14 engines)
A10/A12/A14/A15, L16/L18/L20B/L24/L28, CA18DET, SR20DET, RB25DET, RB26DETT, VQ35DE

### Alfa Romeo (8 engines)
Twin Spark 1.6/1.8/2.0, Nord 1.6/1.8/2.0, Busso V6 2.5/3.0

## Technical Basis

Based on Weber carburetor technical specifications and period tuning guides from:
- 240260280.com DCOE Theory & Tuning
- Dave Andrews carburetor tuning guides

The calculator uses Weber baseline formulas for main and air corrector jets, then layers on heuristics for altitude, cam profile, venturi suggestion, supporting jet choices, and progressive-carb staging. Cam choice now has a stronger effect on choke suggestion, idle/progression fuel, pump delivery, and high-RPM air correction. For DCOE and IDF layouts, the venturi and main-jet baseline is surfaced explicitly as a per-venturi recommendation so single, twin, and triple setups are easier to sanity-check. The setup selector also enforces a basic physical limit: you cannot choose a layout with more venturis than the engine has cylinders or rotors.

## Disclaimer

These are starting recommendations only. Final tuning requires dyno testing or wideband O2 sensor verification.

## License

Released under the MIT License. See `LICENSE` for the full text.

---
Built: March 2026
