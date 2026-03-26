---
title: Align
parent: "Placement Operations"
grand_parent: "Operations"
nav_order: 1
---
# Align

Align precisely positions objects relative to an anchor object along the X, Y, and Z axes. You can align edges, centers, or origins with optional offsets.

<!-- IMAGE_NEEDED: Screenshot showing two objects being aligned with alignment options visible -->

## How to Use

1. Select two or more objects
2. Apply the **Align** operation from the Placement menu
3. Select which object to use as the **Anchor** (reference object)
4. Set alignment options for each axis

## Parameters

### Per Axis (X, Y, and Z each have the same options)

- **Align** - What part of the moving object(s) to align:
  - **None** - No alignment on this axis
  - **Min** - Align the object's minimum edge (left / front / bottom)
  - **Center** - Align the object's center point
  - **Max** - Align the object's maximum edge (right / back / top)
  - **Origin** - Align to the object's origin point
- **Options** - Enable sub-alignment and offset controls
- **Sub-Align** - What part of the anchor to align to (same options as above)
- **Offset** - Distance offset from the anchor position. Supports [expressions](../../workspace/expressions.md).

## Examples

- **Center two objects on X and Y** - Set X Align = Center and Y Align = Center. Both objects will share the same center point.
- **Stack one object on top of another** - Set Z Align = Min, then enable Z Options and set Z Sub-Align = Max. The bottom of the moving object aligns with the top of the anchor.
- **Offset from an edge** - Align to an edge, then use the Offset to add precise spacing.

## Tips

- The Anchor object stays in place; other objects move to align with it
- You can align on one, two, or all three axes independently
- Use offsets to add precise spacing between aligned objects
- Align is non-destructive -- change the settings at any time to re-align

## Related

- [Fit to Bounds](fit-to-bounds.md) - Scale an object to fit specific dimensions
- [Translate](../transform/translate.md) - Move by a specific distance
- [Grouping](../../workspace/grouping.md) - Group aligned objects to keep them together
