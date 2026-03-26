---
title: Cube
parent: "Primitives"
nav_order: 4
---
# Cube

A rectangular box shape with adjustable width, depth, height, and optional rounded edges. The Cube is one of the most commonly used primitives for building designs.

<!--  Screenshot of a Cube primitive on the workspace -->
![20260318 183230 paste 20260318 183230](https://matterhackers.github.io/MatterCAD_Docs/assets/20260318-183230-paste-20260318-183230.jpg)


## Parameters

- **Width** - Size along the X axis (default: 20mm)
- **Depth** - Size along the Y axis (default: 20mm)
- **Height** - Size along the Z axis (default: 20mm)
- **Round** - Enable rounded edges
- **Radius** - Size of the rounding (visible when Round is enabled)
- **Round Segments** - Smoothness of the rounding, more segments = smoother curves (visible when Round is enabled)

## Tips

- Use a Cube as the starting point for boxes, plates, brackets, and enclosures
- Enable Round for smooth, professional-looking edges
- The Radius cannot exceed half of the smallest dimension
- Combine a Cube with [Subtract](../operations/boolean/subtract.md) to create rectangular cutouts and slots

## Related

- [Cylinder](cylinder.md) - Round column shape
- [Pyramid](pyramid.md) - Tapered four-sided shape
- [Hole](hole.md) - A cube pre-configured for boolean subtraction
