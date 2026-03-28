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
- **Options** - Enable advanced controls for this axis:
  - **From Previous** - Chain alignment through objects in alphabetical order. Each object aligns to the previous one instead of the anchor (see below).
  - **Sub-Align** - What part of the reference object to align to (same options as Align, but inverted -- Min becomes the far edge, Max becomes the near edge)
  - **Offset** - Distance offset from the alignment position. Supports [expressions](../../workspace/expressions.md).

## From Previous (Chained Alignment)

When **From Previous** is enabled on an axis, objects are aligned in a chain rather than all aligning to the anchor:

1. Objects are processed in alphabetical order (matching their tree view order)
2. The first object aligns to the **Anchor** as usual
3. Each subsequent object aligns to the **previous object** in the chain

This is useful for stacking or spacing objects sequentially. Combined with **Sub-Align** and **Offset**, you can create evenly spaced layouts where each object sits next to the previous one.

### Example: Stack objects along Z

1. Set Z Align = Min
2. Enable Z Options
3. Turn on Z From Previous
4. Set Z Sub-Align = Max

The first object aligns its bottom to the anchor's top. The second object aligns its bottom to the first object's top. And so on -- creating a vertical stack.

## Examples

- **Center two objects on X and Y** - Set X Align = Center and Y Align = Center. Both objects will share the same center point.
- **Stack one object on top of another** - Set Z Align = Min, then enable Z Options and set Z Sub-Align = Max. The bottom of the moving object aligns with the top of the anchor.
- **Offset from an edge** - Align to an edge, then use the Offset to add precise spacing.
- **Chain objects along X** - Set X Align = Min, enable X Options, turn on From Previous, and set X Sub-Align = Max. Objects line up end-to-end in alphabetical order.

## Tips

- The Anchor object stays in place; other objects move to align with it
- You can align on one, two, or all three axes independently
- Use offsets to add precise spacing between aligned objects
- From Previous can be enabled independently per axis -- chain on X while centering all on Y
- Align is non-destructive -- change the settings at any time to re-align

## Related

- [Fit to Bounds](fit-to-bounds.md) - Scale an object to fit specific dimensions
- [Translate](../transform/translate.md) - Move by a specific distance
- [Grouping](../../workspace/grouping.md) - Group aligned objects to keep them together
