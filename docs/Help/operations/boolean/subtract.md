---
title: Subtract
parent: "Boolean Operations"
grand_parent: "Operations"
nav_order: 4
---
# Subtract

Subtract cuts one or more shapes out of another, performing a boolean subtraction. Use this to create holes, cutouts, and complex negative shapes.

<!-- AUTO_IMAGE: type=from_mcx file=boolean_subtract -->
![boolean_subtract](https://matterhackers.github.io/MatterCAD_Docs/assets/boolean_subtract.png)

## How to Use

1. Select two or more objects where at least one overlaps with another
2. Click the **Subtract** button in the toolbar
3. In the Properties panel, use the **Part(s) to Subtract** dropdown to select which object(s) should be cut away
4. The selected objects are removed from the remaining objects

The objects you choose as "Part(s) to Subtract" are the cutting tools -- their shape is removed from everything else.

## Parameters

- **Part(s) to Subtract** - Select which child objects act as the cutting shapes. Everything else is the base that gets cut

## Tips

- Position your cutting object so it overlaps with the base object exactly where you want material removed
- You can subtract multiple objects at once by selecting several in the Parts to Subtract dropdown
- To create a through-hole, make sure the cutting object extends completely through the base
- If you need a simple hole, consider using the [Hole](../../primitives/hole.md) primitive which is pre-configured for subtraction
- The cutting objects remain in the design tree so you can adjust their position or size and the subtraction updates

## Related

- [Combine](combine.md) - Merge shapes together instead of cutting
- [Intersect](intersect.md) - Keep only the overlapping volume
- [Subtract and Replace](subtract-and-replace.md) - Subtract and keep both resulting parts
