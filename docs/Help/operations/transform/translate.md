---
title: Translate
parent: "Transform Operations"
grand_parent: "Operations"
nav_order: 4
---
# Translate

Translate moves an object by a specific distance along the X, Y, and/or Z axes. Unlike dragging an object with the mouse, Translate lets you enter exact offset values.

<!-- IMAGE_NEEDED: Screenshot showing the Translate operation properties with X, Y, Z offset fields -->

## How to Use

1. Select an object
2. Apply the **Translate** operation from the Transform menu
3. Enter the desired offset values for X, Y, and Z in the Properties panel

## Parameters

- **X, Y, Z** (Translation) - The distance to move the object along each axis, in millimeters. Supports [expressions](../../workspace/expressions.md) for calculated values.

## Tips

- Use Translate when you need precise, repeatable positioning that you can adjust later
- The translation values are relative to the object's current position -- entering 10 for X moves it 10mm to the right from where it is
- For quick repositioning, you can also drag objects directly in the viewport. See [Editing Objects](../../getting-started/editing-objects.md)

## Related

- [Rotate](rotate.md) - Rotate an object by a specific angle
- [Scale](scale.md) - Resize an object precisely
- [Align](../placement/align.md) - Position objects relative to each other
