---
title: Star Path
parent: "2D Paths"
nav_order: 5
---
# Star Path

A star-shaped 2D path with configurable number of points and inner/outer radius. Use with [Linear Extrude](../operations/path/linear-extrude.md) to create 3D star shapes.

<!-- IMAGE_NEEDED: Screenshot of a Star Path on the workspace -->

## Parameters

- **Points** - Number of star points
- **Outer Radius** - Distance from center to the tip of each point
- **Inner Radius** - Distance from center to the valleys between points

## Tips

- The ratio between Inner and Outer Radius determines how "pointy" the star is. A small Inner Radius creates sharp, pronounced points.
- Set Points to 5 for a classic star, 6 for a Star of David shape, or higher for gear-like shapes
- Use [Smooth Path](../operations/path/smooth-path.md) on a Star Path to create rounded star shapes

## Related

- [Circle Path](circle-path.md) - A smooth circle
- [Gear 2D](../mechanical/gear-2d.md) - A proper gear profile
- [Linear Extrude](../operations/path/linear-extrude.md) - Give paths height
