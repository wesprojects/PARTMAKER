# PARTMAKER

Parametric generator for printable and machinable shop parts — nine part families, watertight STL and STEP out.

---

## Usage

Launch the app at [wesprojects.github.io/PARTMAKER](https://wesprojects.github.io/PARTMAKER).

## Overview

PARTMAKER builds solid geometry from dimensions you enter. Every part is generated as a closed manifold mesh and checked before export, and the app reports the fits, clearances and wall thicknesses it produced so you can see what you are about to print.

## Part families

| Family | What it makes |
|---|---|
| **End plug** | Plugs for tube ends. Round, oval, square, rect. Grip ribs, relief slots, taper, chamfers. |
| **End cap** | Caps that fit over a part. Sized from the part's own outside dimension. |
| **Chair tip** | End plug with a flat or angled base, so a raked leg still sits square. Rotate or skew. |
| **Hole plug** | Blind-hole plugs and shelf pins. Sized from the hole. |
| **Spacer / washer** | Cylindrical or hex spacers, and flat washers. |
| **Hose adapter** | Vacuum and dust-extraction adapters. Male or female per end, optional coarse hose threads, left or right hand. |
| **Cable grommet** | Four-piece desk grommet: liner, cap, brush, nut. Snap-in or threaded mounting; snap-groove or bayonet cap. |
| **Spray stencil** | Flat stencils cut from true stencil typefaces. Splits across build plates with keyed joints. |
| **Air vent** | Wall and duct vents. Fixed louvers, five printed mesh patterns, or a print-in-place backdraft damper. |

## Features

**Geometry**
- Closed manifold output, verified by edge pairing and signed volume
- Helical threads, bayonet channels, print-in-place hinges
- Multi-part models exported as separate solids

**Output**
- Binary STL with unit recorded in the header
- STEP AP214 faceted B-rep, planar faces preserved where the geometry allows
- Files named `model-product-date`

**Working**
- Live 3D preview with cutaway and wireframe
- Millimetres or inches, lossless either way
- 63 presets drawn from published standards — ISO 7089, SAE and USS washers, ISO 273 clearance holes, standard hose and duct sizes
- Save, load, undo and redo

**Checks**
Every build is validated before you print it. The app reports interference and clearance, wall thicknesses below two perimeters, features that would break through a wall, overhangs that need support, and print orientation.

## Notes

Presets are starting points sized from published standards, not substitutes for measuring the part in front of you. Hose threads in particular are not standardised between manufacturers — measure yours before committing to a long print.
