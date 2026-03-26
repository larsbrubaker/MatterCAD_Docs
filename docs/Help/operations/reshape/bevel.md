---
title: Bevel
parent: "Reshape Operations"
grand_parent: "Operations"
nav_order: 1
---
# Bevel

Bevel rounds or chamfers a selected edge of an object by performing a boolean cut with a shaped profile. This adds a smooth, professional-looking transition between faces.

<!-- IMAGE_NEEDED: Before and after showing a cube with one edge beveled to a smooth round -->

## How to Use

1. Select an object
2. Apply the **Bevel** operation from the Reshape menu
3. Select which edge to bevel
4. Adjust the angles, radius, and number of sides

## Parameters

- **Edge to Bevel** - Select which edge of the object to round (edges are numbered, wraps around if out of bounds)
- **Start Angle** - The angle to cut on the starting side (default: 45 degrees)
- **End Angle** - The angle to cut on the ending side (default: 45 degrees)
- **Radius** - The size of the bevel arc (default: 2mm). Larger values create a wider, more gradual round
- **Sides** - The number of segments in the bevel arc (default: 8). More sides = smoother round

## Tips

- Equal Start and End Angles create a symmetric bevel
- Set Sides to 1 for a simple chamfer (flat cut) instead of a smooth round
- Increase Radius for a more pronounced rounding effect
- Bevel is computed as a boolean operation, so it may take a moment on complex geometry

## Related

- [Hollow Out](hollow-out.md) - Create a shell from a solid
- [Plane Cut](plane-cut.md) - Cut with a flat plane
- [Cube](../../primitives/cube.md) - Cubes have a built-in Round option for simple edge rounding
