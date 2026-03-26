---
title: Linear Array
parent: "Array Operations"
grand_parent: "Operations"
nav_order: 2
---
# Linear Array

Linear Array creates multiple copies of an object arranged in a straight line along a specified direction. Use this for creating repeating features like bolt holes, teeth, slots, or fence posts.

<!-- AUTO_IMAGE: type=from_mcx file=array_linear -->
![array_linear](https://matterhackers.github.io/MatterCAD_Docs/assets/array_linear.png)

## How to Use

1. Select an object
2. Apply the **Linear Array** operation from the Array menu
3. Set the number of copies, direction, and spacing

## Parameters

- **Count** - Number of copies to create (default: 3, range: 2-10). Supports [expressions](../../workspace/expressions.md).
- **Direction** - The axis direction for the array. Default is along the X axis (left to right). You can set any direction vector.
- **Distance** - Space between copies in millimeters (default: 30mm). Supports [expressions](../../workspace/expressions.md).

## Tips

- The first copy stays at the original position. Additional copies are placed at 1x, 2x, 3x the distance along the direction
- Change the Direction vector to array along any angle, not just the main axes
- Use expressions for Count or Distance to create parametric patterns that adapt when you change values

## Related

- [Radial Array](radial-array.md) - Arrange copies in a circular pattern
- [Advanced Array](advanced-array.md) - Create arrays with rotation and scaling per copy
