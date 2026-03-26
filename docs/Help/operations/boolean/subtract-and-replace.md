---
title: Subtract and Replace
parent: "Boolean Operations"
grand_parent: "Operations"
nav_order: 3
---
# Subtract and Replace

Subtract and Replace performs a boolean subtraction but keeps both resulting parts -- the base with the cutout, and the piece that was cut away. This is useful for creating multi-part designs or color-separated objects.

<!-- AUTO_IMAGE: type=from_mcx file=boolean_subtract_and_replace -->
![boolean_subtract_and_replace](https://matterhackers.github.io/MatterCAD_Docs/assets/boolean_subtract_and_replace.png)

## How to Use

1. Select two or more overlapping objects
2. Click the **Subtract and Replace** button in the toolbar
3. In the Properties panel, use **Part(s) to Subtract and Replace** to select the cutting objects
4. The result contains both the subtracted base and the intersection piece as separate child objects

## Parameters

- **Part(s) to Subtract and Replace** - Select which child objects act as the cutting shapes

## When to Use This

- **Multi-color designs** - Split an object at color boundaries so each part can have a different color or material
- **Assembly design** - Create interlocking parts that fit together precisely
- **Inlay work** - Cut a shape from a base and keep the cutout as a separate insertable piece

## Tips

- Unlike regular [Subtract](subtract.md), this operation creates both the subtraction result and the intersection result as children
- Both resulting parts fit together perfectly since they were cut from the same boolean operation
- You can assign different colors to each resulting part for multi-material designs

## Related

- [Subtract](subtract.md) - Cut a shape away without keeping the removed piece
- [Combine](combine.md) - Merge shapes together
- [Intersect](intersect.md) - Keep only the overlapping volume
