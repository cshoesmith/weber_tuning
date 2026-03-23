# Weber Carburetor Jetting Calculator v3

A standalone Weber carburetor jetting calculator built around baseline Weber formulas plus conservative tuning heuristics for DCOE, IDF, and 32/36 progressive setups.

## Features

- **61 Engine Database**: Toyota, Honda, Mazda, Nissan/Datsun, Alfa Romeo (1960-2010)
- **Multiple Weber Families**: DCOE sidedraft, IDF downdraft, and 32/36 progressive baselines
- **Setup Selector**: DCOE single/twin/triple, IDF single/twin, and 32/36 progressive single
- **Stronger Cam Modeling**: Stock, street, and race cams now shift venturi suggestions plus main, idle, pump, and air-corrector baselines more noticeably
- **Setup Preview**: Recommendations now begin with the selected carb setup, a visual illustration, and per-venturi/per-barrel load context
- **Configuration Health Score**: Enforce the choke/jet sizes you actually have, then see whether the remaining circuits can compensate or whether the combo is a poor fit
- **Body-Specific Choke Availability**: DCOE and IDF venturi choices now change with carb body size so unrealistic pairings are filtered out up front
- **Baseline Weber Formulas**: Family-specific main and air correction rules, plus idle/emulsion/needle starting points
- **Supports**: 4-cyl, 6-cyl, and rotary engines (985cc - 3500cc)
- **Configurations**: DCOE single/twin/triple, IDF single/twin, and 32/36 progressive single
- **Auto-venturi**: Suggests appropriate choke size based on displacement and approximate stock peak-power RPM
- **About Button**: Shows project contact details, MIT license information, and a donation placeholder button
- **Reference Tables Button**: Opens all lookup tables and advisory material directly from the main page
- **Reference Links Button**: Opens source links formatted in Chicago-style bibliography form

## Usage

1. Open `index.html` or `weber_calculator.html` in any web browser
2. Select your vehicle make from the first dropdown
3. Select your engine from the connected engine dropdown (auto-fills specs)
4. Confirm the cam profile for the engine or your build
5. The calculator suggests a carburetor setup after the cam choice; keep it or override it manually
6. Override displacement/RPM and adjust carb body, venturi, and supporting settings as needed
7. If you only have certain jets on hand, enter them in the available-parts override fields and review the Configuration Health Score
8. Recommendations update live as settings change, with a brief visual highlight when the calculated results change

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

The calculator uses Weber baseline formulas for main and air corrector jets, then layers on heuristics for altitude, cam profile, venturi suggestion, supporting jet choices, and progressive-carb staging. Cam choice now has a stronger effect on choke suggestion, idle/progression fuel, pump delivery, and high-RPM air correction. For DCOE and IDF layouts, the venturi and main-jet baseline is surfaced explicitly as a per-venturi recommendation so single, twin, and triple setups are easier to sanity-check.

## Disclaimer

These are starting recommendations only. Final tuning requires dyno testing or wideband O2 sensor verification.

## License

Released under the MIT License. See `LICENSE` for the full text.

---
Built: March 2026
