---
title: Rotate
parent: "Transform Operations"
grand_parent: "Operations"
nav_order: 2
---
# Rotate

Rotate turns an object around a specified axis by a given angle. You can rotate around any axis direction and choose the center point of rotation.

<!-- IMAGE_NEEDED: Screenshot showing the Rotate operation with the rotation gizmo visible in the viewport -->

## How to Use

1. Select an object
2. Apply the **Rotate** operation from the Transform menu
3. Set the rotation angle and axis in the Properties panel

You can also rotate objects directly in the viewport by clicking the rotate corner controls on a selected object. Moving your mouse over the angle indicators snaps to 45-degree increments.

## Parameters

- **Angle** - The rotation angle in degrees (range: 3-360). Supports [expressions](../../workspace/expressions.md).
- **Rotate About** - Defines the axis of rotation and the origin point. You can rotate around the X, Y, or Z axis, or specify a custom direction.

## Tips

- The rotation is centered on the object's bounding box center by default
- For 90-degree rotations, the snap indicators make it easy to get exact values
- Use the Rotate operation (rather than viewport controls) when you need a precise angle that isn't a multiple of 45 degrees
- You can change the rotation axis after applying the operation by editing the Rotate About property

## Related

- [Translate](translate.md) - Move an object by a specific distance
- [Scale](scale.md) - Resize an object
- [Mirror](mirror.md) - Create a mirrored reflection
