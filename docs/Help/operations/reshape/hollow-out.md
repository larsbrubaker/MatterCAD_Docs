---
title: Hollow Out
parent: "Reshape Operations"
grand_parent: "Operations"
nav_order: 3
---
# Hollow Out

Hollow Out creates a hollow shell from a solid object by offsetting the surface inward. The result is a thin-walled version of the original shape.

<!-- IMAGE_NEEDED: Cross-section view showing a solid object hollowed out with visible wall thickness -->

## How to Use

1. Select a solid object
2. Apply the **Hollow Out** operation from the Reshape menu
3. Set the desired wall thickness

## Parameters

- **Distance** - The wall thickness in millimeters (default: 2mm). This is how thick the resulting shell will be.
- **Num Cells** - Resolution of the hollowing algorithm (default: 64). Higher values create smoother internal surfaces but take longer to compute.

## Tips

- Hollow Out is useful for creating enclosures, containers, vases, and lightweight parts
- A wall thickness of 1-2mm is typical for most 3D-printed parts
- Increase Num Cells if the internal surface appears rough or blocky
- The hollowing creates an open bottom -- combine with a [Cube](../../primitives/cube.md) if you need a closed base
- For complex shapes, the computation may take a few seconds

## Related

- [Plane Cut](plane-cut.md) - Cut an object at a specific height
- [Bevel](bevel.md) - Round edges of an object
- [Subtract](../boolean/subtract.md) - Manually cut material away
