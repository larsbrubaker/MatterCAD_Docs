---
title: Combine
parent: "Boolean Operations"
grand_parent: "Operations"
nav_order: 1
---
# Combine

Combine merges multiple objects into a single unified solid. This is equivalent to a boolean union operation -- it joins overlapping shapes into one continuous mesh.

<!-- AUTO_IMAGE: type=from_mcx file=boolean_combine -->
![boolean_combine](https://matterhackers.github.io/MatterCAD_Docs/assets/boolean_combine.png)

## How to Use

1. Select two or more objects that overlap
2. Click the **Combine** button in the toolbar, or find it under the Boolean operations menu
3. MatterCAD merges all selected objects into a single shape

The result is one solid object where all the individual shapes have been joined together. Any internal faces where objects overlapped are removed.

## Tips

- Objects must overlap for Combine to produce a meaningful result. If objects don't touch, they will still be joined into one mesh but remain visually separate
- Combine automatically handles Hole objects -- any objects marked as holes are subtracted rather than added
- If the result looks incorrect, make sure all source objects are valid (watertight) meshes. Use [Repair](../mesh/repair.md) on imported models first
- Combine preserves per-face colors from the original objects

## Related

- [Subtract](subtract.md) - Cut one shape out of another
- [Intersect](intersect.md) - Keep only overlapping volume
- [Subtract and Replace](subtract-and-replace.md) - Subtract and keep both parts
