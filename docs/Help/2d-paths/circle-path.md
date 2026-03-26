---
title: Circle Path
parent: "2D Paths"
nav_order: 2
---
# Circle Path

A circular 2D path. Use with [Linear Extrude](../operations/path/linear-extrude.md) to create cylinders, or [Revolve](../operations/path/revolve.md) to create torus-like shapes.

<!-- IMAGE_NEEDED: Screenshot of a Circle Path on the workspace -->

## Parameters

- **Diameter** - The diameter of the circle (default: 20mm)
- **Segments** - Number of line segments forming the circle. More = smoother

## Tips

- A Circle Path combined with Linear Extrude produces a cylinder, similar to the [Cylinder](../primitives/cylinder.md) primitive but with more flexibility in how you build up from it
- Use as a base for Revolve to create ring shapes

## Related

- [Box Path](box-path.md) - A rectangular 2D path
- [Ring Path](ring-path.md) - A circle with a hole
- [Linear Extrude](../operations/path/linear-extrude.md) - Give paths height
