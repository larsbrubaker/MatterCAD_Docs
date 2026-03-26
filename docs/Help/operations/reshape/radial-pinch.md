---
title: Radial Pinch
parent: "Reshape Operations"
grand_parent: "Operations"
nav_order: 6
---
# Radial Pinch

Radial Pinch compresses an object inward from a center point with a customizable profile curve. Unlike regular [Pinch](pinch.md) which works from back to front, Radial Pinch compresses symmetrically around a center axis.

<!-- IMAGE_NEEDED: Before and after showing an object with radial pinch applied, creating a waisted shape -->

## How to Use

1. Select an object
2. Apply the **Radial Pinch** operation from the Reshape menu
3. Edit the path profile to define how much pinch is applied at each height
4. Adjust the number of slices for smoothness

## Parameters

- **Path** - A profile curve editor that defines the pinch amount at each height level. Edit the curve to create custom pinch profiles
- **Pinch Slices** - Number of vertical cuts for smooth pinching. More slices = smoother results

### Advanced Parameters

- **Pinch Type** - Direction of compression:
  - **Radial** - Compress equally from all sides toward center
  - **X Axis** - Compress only along the X axis
  - **Y Axis** - Compress only along the Y axis
- **Rotation Offset** - Shift the center of the pinch effect

## Tips

- Use the path editor to create hourglass, bottle, or vase-like shapes
- Radial pinch is ideal for creating organic, rounded forms from cylindrical objects
- Increase Pinch Slices for smoother curves, especially on tight pinch profiles

## Related

- [Pinch](pinch.md) - Simple back-to-front compression
- [Twist](twist.md) - Spiral rotation along height
- [Curve](curve.md) - Bend into an arc
