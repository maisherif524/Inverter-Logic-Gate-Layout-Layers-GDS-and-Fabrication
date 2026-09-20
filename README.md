# Logic Gate Layout, Layers, GDS & Fabrication 

Full-custom layout of a CMOS inverter in the TSMC N65 PDK using Cadence Virtuoso, verified with Calibre DRC/LVS.

## What's covered

**Part 1 – Inverter design & verification (`inv01`)**
- Schematic with `pch_lvt` / `nch_lvt` devices
- Layout in Layout XL, optimized for area, with substrate/N-well straps (M1+PP for NMOS, M1+NP+NW for PMOS) for latch-up protection
- DRC and LVS clean-up, with final reports

**Part 2 – Layer analysis**
- Exploring PDK layers with the Layer Palette and `display.drf`
- Mapping layers and their logical operations to masks and fabrication steps

**Part 3 – GDS export/import & migration (`inv03`)**
- Stream-out of `inv01` and stream-in with a modified layer map file
- LVT → HVT migration (`pch_hvt` / `nch_hvt`) without redrawing the layout

## Repository structure
- `schematics/` – schematic screenshots
- `layout/` – layout screenshots 
- `reports/` – DRC summary and LVS reports
- `layer_map/` – original and modified layer map files
- `report.pdf` – full lab report

## Tools
Cadence Virtuoso (Schematic, Layout XL) · Siemens Calibre (DRC/LVS) · TSMC N65 PDK
