# Weber Carburetor Jetting Calculator v3

A standalone Weber carburetor jetting calculator built around baseline Weber formulas plus conservative tuning heuristics for DCOE, IDF, and 32/36 progressive setups.

## Features

- **61 Engine Database**: Toyota, Honda, Mazda, Nissan/Datsun, Alfa Romeo (1960-2010)
- **Multiple Weber Families**: DCOE sidedraft, IDF downdraft, and 32/36 progressive baselines
- **Setup Selector**: DCOE single/twin/triple, IDF single/twin, and 32/36 progressive single
- **Baseline Weber Formulas**: Family-specific main and air correction rules, plus idle/emulsion/needle starting points
- **Supports**: 4-cyl, 6-cyl, and rotary engines (985cc - 3500cc)
- **Configurations**: DCOE single/twin/triple, IDF single/twin, and 32/36 progressive single
- **Auto-venturi**: Suggests appropriate choke size based on displacement and peak RPM
- **Reference Tables Button**: Opens all lookup tables and advisory material directly from the main page

## Usage

1. Open `weber_dcoe_calculator.html` in any web browser
2. Select your vehicle make from the first dropdown
3. Select your engine from the connected engine dropdown (auto-fills specs)
4. Override displacement/RPM if modified
5. Choose the carburetor setup you want to model
6. Adjust carb body, venturi, and supporting settings as needed
7. Get instant baseline jetting recommendations

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

The calculator uses Weber baseline formulas for main and air corrector jets, then layers on conservative heuristics for altitude, cam profile, venturi suggestion, supporting jet choices, and progressive-carb staging.

## Disclaimer

These are starting recommendations only. Final tuning requires dyno testing or wideband O2 sensor verification.

---
Built: March 2026
