---
title: Curve
parent: "Reshape Operations"
grand_parent: "Operations"
nav_order: 2
---
# Curve

Curve bends a straight object into an arc or circular shape. You can control the bend by specifying either an angle or a diameter to wrap around.

<!-- IMAGE_NEEDED: Before and after showing a straight bar being curved into an arc -->

## How to Use

1. Select an object
2. Apply the **Curve** operation from the Reshape menu
3. Choose between Angle or Diameter bend type
4. Adjust the parameters to get the desired curvature

## Parameters

- **Bend Type** - Choose between:
  - **Angle** - Specify the bend angle directly (1-360 degrees)
  - **Diameter** - Specify the diameter of the circle the part wraps around
- **Bend Direction** - Bend Up or Bend Down
- **Start Percent** - Where along the object to start the bend (0-100%)
- **Split Mesh** - Split the mesh for smooth curves (default: on)
- **Min Sides Per Rotation** - Minimum number of mesh segments per full revolution. Higher values = smoother curves

### Advanced Parameters

- **Start Bend Percent** - Percentage from the left where the bend starts
- **End Bend Percent** - Percentage from the left where the bend ends

## Tips

- Use Curve to create arches, rings, and bent brackets from straight stock shapes
- Setting the angle to 360 wraps the object into a complete ring
- Increase Min Sides Per Rotation for smoother results on tight bends
- The object is bent along its length (X axis)

## Related

- [Twist](twist.md) - Rotate along height instead of bending
- [Torus](../../primitives/torus.md) - A ready-made ring shape
