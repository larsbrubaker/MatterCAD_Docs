---
title: Ring Path
parent: "2D Paths"
nav_order: 4
---
# Ring Path

A 2D ring shape -- a circle with a circular hole in the center. Use with [Linear Extrude](../operations/path/linear-extrude.md) to create tube or washer shapes.

<!-- IMAGE_NEEDED: Screenshot of a Ring Path on the workspace -->

## Parameters

- **Outer Diameter** - The outer diameter of the ring
- **Inner Diameter** - The diameter of the hole in the center

## Tips

- The wall thickness of the ring is (Outer Diameter - Inner Diameter) / 2
- Extruding a Ring Path creates a tube similar to the [Ring](../primitives/ring.md) primitive

## Related

- [Circle Path](circle-path.md) - A solid circle (no hole)
- [Ring](../primitives/ring.md) - A ready-made 3D tube shape
- [Linear Extrude](../operations/path/linear-extrude.md) - Give paths height
