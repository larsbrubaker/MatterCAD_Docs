---
title: Intersect
parent: "Boolean Operations"
grand_parent: "Operations"
nav_order: 2
---
# Intersect

Intersect keeps only the volume where two or more objects overlap, discarding everything else. This is useful for creating shapes that conform to the boundaries of multiple objects.

<!-- AUTO_IMAGE: type=from_mcx file=boolean_intersect -->
![boolean_intersect](https://matterhackers.github.io/MatterCAD_Docs/assets/boolean_intersect.png)

## How to Use

1. Select two or more overlapping objects
2. Click the **Intersect** button in the toolbar
3. MatterCAD calculates the overlapping volume and creates a new shape from it

Only the region that exists in all selected objects is kept. Everything outside the overlap is removed.

## Tips

- Objects must actually overlap for Intersect to produce a result. If there is no overlap, the result will be empty
- Intersect works sequentially when more than two objects are selected -- first two are intersected, then the result is intersected with the third, and so on
- This operation is useful for trimming objects to fit within a specific boundary shape
- Intersect preserves per-face colors from the original objects

## Related

- [Combine](combine.md) - Merge shapes together
- [Subtract](subtract.md) - Cut one shape from another
- [Plane Cut](../reshape/plane-cut.md) - Cut with a flat plane instead of another shape
