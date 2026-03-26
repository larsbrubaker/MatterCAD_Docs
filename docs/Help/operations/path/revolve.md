---
title: Revolve
parent: "Path Operations"
grand_parent: "Operations"
nav_order: 6
---
# Revolve

Revolve spins a 2D path around an axis to create a 3D solid of revolution. This is how you create vases, bowls, wheels, and other rotationally symmetric objects.

<!-- IMAGE_NEEDED: Before and after showing a profile path being revolved into a vase shape -->

## How to Use

1. Select a 2D path
2. Apply **Revolve** from the Path operations menu
3. Adjust the rotation range, axis position, and number of sides

## Parameters

- **Rotation** - Total rotation angle for the revolve (default: 0, range: 0-360). Set to 360 for a complete revolution.
- **Axis Position** - Offset of the rotation axis from the path center (default: 0, range: -30 to 30). Positive moves the axis away from the path, creating a larger opening.
- **Starting Angle** - Where the revolution begins (default: 0)
- **Ending Angle** - Where the revolution ends (default: 45). Set to 360 for a full revolution.
- **Sides** - Number of segments around the revolution (default: 30). More = smoother surface.

## Tips

- Use Axis Position to control the inner diameter of the revolved shape
- Set Starting and Ending Angle to less than 360 to create partial revolutions (arches, gutters)
- Draw a profile path of your vase or bowl shape, then revolve it for perfect symmetry
- A [Circle Path](../../2d-paths/circle-path.md) revolved creates a torus

## Related

- [Linear Extrude](linear-extrude.md) - Extrude straight up instead of revolving
- [2D Paths](../../2d-paths/index.md) - Create profile paths to revolve
- [Torus](../../primitives/torus.md) - A ready-made revolved ring shape
