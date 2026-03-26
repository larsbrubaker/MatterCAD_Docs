---
title: Twist
parent: "Reshape Operations"
grand_parent: "Operations"
nav_order: 7
---
# Twist

Twist rotates the top of an object relative to the bottom, creating a spiral or twisted effect along the height. The rotation progresses smoothly from bottom to top.

<!-- IMAGE_NEEDED: Before and after showing a cube being twisted into a spiral column -->

## How to Use

1. Select an object
2. Apply the **Twist** operation from the Reshape menu
3. Set the twist angle and adjust slicing for smoothness

## Parameters

- **Rotation Type** - Choose between:
  - **Angle** - Specify the total twist angle in degrees (3-360)
  - **Distance** - Specify the twist as a distance along the circumference
- **Rotation Slices** - Number of vertical cuts added for smooth twisting. More slices = smoother twist
- **Twist Cw** - Direction of twist: right (clockwise) or left (counterclockwise)

### Advanced Parameters

- **Edit Radius** - Override the automatic radius calculation
- **Override Radius** - Custom radius for the twist calculation
- **Easing Type** - How the twist accelerates (Linear, Cubic, etc.)
- **Easing Option** - Easing direction (In, Out, InOut)
- **Start Height Percent** - Where along the height to start twisting (0-100%)
- **End Height Percent** - Where along the height to stop twisting (0-100%)
- **Rotation Offset** - Shift the center of rotation

## Tips

- Higher Rotation Slices values produce smoother results but generate more geometry
- Use Start and End Height Percent to twist only a portion of the object
- A 90-degree twist on a square column creates an elegant architectural effect
- Try different easing types for non-uniform twist distributions

## Related

- [Curve](curve.md) - Bend an object into an arc
- [Pinch](pinch.md) - Compress toward center
