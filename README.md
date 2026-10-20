# Perixx PERIBOARD-524 3D Models

Parametric OpenSCAD 3D models and key measurement annotations for the **Perixx PERIBOARD-524** ergonomic split keyboard.

## Overview

This project provides 3D models designed for 3D printing (e.g., using flexible TPU filament) custom keyboard covers, key dampeners, or spacer guards matching the split layout of the Perixx PERIBOARD-524.

## Files

- **`keyboard_left.scad`**: OpenSCAD model for the left half of the keyboard.
- **`keyboard_right.scad`**: OpenSCAD model for the right half of the keyboard.
- **`keyboard_left_measured.json` / `keyboard_right_measured.json`**: Key polygon coordinates measured with VGG Image Annotator (VIA).
- **`keyboard_left_calibration.json` / `keyboard_right_calibration.json`**: Image calibration metadata used to convert pixels to millimeter dimensions.

## Requirements & Usage

### OpenSCAD

To preview or export models to STL:

1. Open [OpenSCAD](https://openscad.org/).
2. Load `keyboard_left.scad` or `keyboard_right.scad`.
3. Press **F5** to preview or **F6** to render.
4. Export to STL via **File > Export as STL...** or using the CLI:

```bash
openscad -o keyboard_left.stl keyboard_left.scad
openscad -o keyboard_right.stl keyboard_right.scad
```

### Printing Recommendations

- **Material**: TPU / flexible filament for a snug, flexible fit over keys and case edges.
- **Layer Height**: 0.2 mm (or 0.15 mm for finer detail).
- **Infill**: 100% or high infill for structural durability.
