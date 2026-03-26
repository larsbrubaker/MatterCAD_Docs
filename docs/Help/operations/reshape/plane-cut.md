---
title: Plane Cut
parent: "Reshape Operations"
grand_parent: "Operations"
nav_order: 5
---
# Plane Cut

Plane Cut slices an object at a specified height with a horizontal plane, keeping only the portion below the cut. The cut surface is capped with a flat face.

<!-- IMAGE_NEEDED: Before and after showing an object being sliced at a specific height -->

## How to Use

1. Select an object
2. Apply the **Plane Cut** operation from the Reshape menu
3. Set the cut height

## Parameters

- **Cut Height** - The Z height at which to slice the object (default: 10mm, range: 1-200mm)

## Tips

- Use Plane Cut to flatten the top of a model at a specific height
- Useful for trimming imported models or creating flat bases
- For cutting with a non-planar shape, use [Subtract](../boolean/subtract.md) with another object instead
- For cutting with a tilted plane, rotate the object first, apply Plane Cut, then rotate back

## Related

- [Intersect](../boolean/intersect.md) - Keep only where objects overlap
- [Subtract](../boolean/subtract.md) - Cut with any shape, not just a plane
- [Hollow Out](hollow-out.md) - Create a hollow shell
