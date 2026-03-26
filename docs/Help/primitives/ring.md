---
title: Ring
parent: "Primitives"
nav_order: 13
---
# Ring

A hollow cylinder (tube) with independent inner and outer diameters and a specified height. Also known as a pipe or tube shape.

<!--  Screenshot of a Ring primitive on the workspace -->
![20260318 183848 paste 20260318 183848](https://matterhackers.github.io/MatterCAD_Docs/assets/20260318-183848-paste-20260318-183848.jpg)


## Parameters

- **Outer Diameter** - The outside width of the ring (default: 20mm)
- **Inner Diameter** - The diameter of the hollow center (default: 15mm)
- **Height** - How tall the ring is (default: 5mm)
- **Sides** - Number of segments around the perimeter (default: 40)

### Advanced Parameters

Enable **Advanced** mode for additional controls:

- **Starting Angle** - Angle where the ring begins (default: 0)
- **Ending Angle** - Angle where the ring ends (default: 360). Set less than 360 for a partial ring
- **Round** - Add rounding to the edges (None, Up, or Down)
- **Direction** - Round toward the inner or outer edge (visible when Round is enabled)
- **Round Segments** - Smoothness of the rounding (visible when Round is enabled)

## Tips

- The wall thickness equals (Outer Diameter - Inner Diameter) / 2
- Use this for washers, spacers, bushings, and tube-like features
- Set the height tall for pipes or short for flat washers
- Use Starting and Ending Angles for partial ring shapes like C-clips

## Related

- [Torus](torus.md) - A donut-shaped ring with a round cross-section
- [Cylinder](cylinder.md) - A solid round column (no hollow center)
