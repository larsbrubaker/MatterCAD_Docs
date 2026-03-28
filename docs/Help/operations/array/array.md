---
title: Array
parent: "Array Operations"
grand_parent: "Operations"
nav_order: 1
---
# Array

Array creates multiple copies of an object with configurable offset, rotation, scale, and randomization. You can create simple linear rows, circular patterns, spirals, and complex progressive arrangements -- all from one operation.

<!-- IMAGE_NEEDED: Screenshot of the Array operation panel showing the main parameters -->

## How to Use

1. Select an object
2. Apply the **Array** operation from the Duplication menu
3. Adjust offset, count, and optionally enable rotation, scale, or randomization

## Count

Controls how many copies are created and how they are distributed.

- **Fit Type** - Choose how count is determined:
  - **Fixed Count** - You specify an exact number of copies
  - **Fit Length** - Copies fill a total length, count is calculated automatically
  - **Fit Curve** - Copies are distributed along a sibling 3D Curve object
- **Count** - Number of copies (shown for Fixed Count). Supports [expressions](../../workspace/expressions.md).
- **Fit Length** - Total length to fill in mm (shown for Fit Length). Supports [expressions](../../workspace/expressions.md).
- **Curve Id** - Name or ID of a sibling curve to follow (shown for Fit Curve)

## Offset

Controls spacing and direction between copies.

- **Offset Method**:
  - **Relative** - Offset is multiplied by the object's bounding box size. A value of (1, 0, 0) places each copy one object-width apart along X.
  - **Constant** - Offset is a fixed distance in mm regardless of object size.
- **Offset** - The X, Y, Z offset vector between copies

## Rotation

Enable the **Use Rotation** toggle to add rotation to each copy.

- **Rotation Angle** - Degrees of rotation. Supports [expressions](../../workspace/expressions.md).
- **Angle Mode**:
  - **Per Copy** - Each copy rotates this many degrees relative to the previous copy
  - **Total** - The rotation angle is spread evenly across all copies
- **Rotate About** - The axis and center point of rotation. Drag the origin in the viewport to change the radius of circular patterns.
- **Rotate Part** - When on, each copy's geometry rotates to match its position (like spokes on a wheel). When off, copies maintain their original orientation.

## Scale

Enable the **Use Scale** toggle to progressively scale copies.

- **Scale** - Per-axis scale multiplier applied at each step. Values less than 1 shrink copies; greater than 1 grow them.
- **Scale Offset** - When on, the offset distance also scales with each step, creating tightening spirals or converging patterns.

## Randomize

Enable the **Use Randomize** toggle to add variation to copies.

- **Random Offset** - Maximum random position offset per axis in mm
- **Random Rotation** - Maximum random rotation per axis in degrees
- **Random Scale Range** - Maximum random scale variation per axis (e.g., 0.1 means +/-10%)
- **Random Seed** - Change this value to get a different random arrangement. Supports [expressions](../../workspace/expressions.md).
- **Exclude First** - Keep the first copy at its exact computed position (default: on)

## Common Patterns

### Linear Array
Leave rotation and scale off. Set Offset Method to Relative with offset (1, 0, 0) for copies spaced one object-width apart along X. Adjust the offset vector to change direction and spacing.

### Radial Array
Enable Use Rotation, set Rotation Angle to 360/count, and adjust the Rotate About origin to set the circle radius. Turn on Rotate Part for spoke-like arrangements.

### Spiral
Enable both rotation and scale. Set a rotation angle and a scale less than 1.0 with Scale Offset on. Copies will spiral inward.

### Staircase
Set Offset to (1, 0, 0.5) for horizontal spacing with vertical rise. Enable rotation with a small angle for a curving staircase.

## Tips

- The first copy stays at the original position; additional copies are offset from there
- Use expressions for Count, Rotation Angle, or Fit Length to create parametric patterns
- Relative offset is usually easier to work with since it adapts when you resize the source object
- Drag the rotation axis origin in the viewport to interactively adjust circular pattern radius

## Related

- [Align](../placement/align.md) - Position objects relative to each other
- [Select Child](select-child.md) - Pick a specific copy from the array
