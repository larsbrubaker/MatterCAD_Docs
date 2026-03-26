---
title: Reduce
parent: "Mesh Operations"
grand_parent: "Operations"
nav_order: 1
---
# Reduce (Decimate)

Reduce lowers the polygon count of a mesh while preserving the overall shape. This is useful for simplifying highly detailed models, reducing file size, and speeding up operations on complex geometry.

![20260324 080430 paste 20260324 080430](https://matterhackers.github.io/MatterCAD_Docs/assets/20260324-080430-paste-20260324-080430.jpg)


## How to Use

1. Select an object
2. Apply the **Reduce** operation from the Mesh menu
3. Choose your target (count or percentage) and adjust

## Parameters

- **Mode** - Choose how to specify the target:
  - **Percent** - Keep a percentage of the original polygons (default: 50%)
  - **Count** - Target a specific polygon count
- **Source Polygon Count** - Original number of polygons (read only)
- **Target Percent** - Percentage of polygons to keep (visible in Percent mode)
- **Target Count** - Exact number of polygons to keep (visible in Count mode)
- **Count After Percent Reduction** - Final polygon count after percentage reduction (read only)
- **Maintain Surface** - Project vertices back to the original surface for higher accuracy (slower but more faithful to the original shape)

## Tips

- 50% reduction usually preserves visual quality well
- Enable Maintain Surface when accuracy matters more than speed
- Reducing polygon count speeds up boolean operations on complex imported models
- Very low polygon counts will visibly degrade the shape -- check the result before committing

## Related

- [Repair](repair.md) - Fix mesh problems
