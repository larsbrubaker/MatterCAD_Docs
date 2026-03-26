---
title: Sphere
parent: "Primitives"
nav_order: 14
---
# Sphere

A round ball shape with adjustable diameter and detail level.

<!--  Screenshot of a Sphere primitive on the workspace -->
![20260318 183909 paste 20260318 183909](https://matterhackers.github.io/MatterCAD_Docs/assets/20260318-183909-paste-20260318-183909.jpg)


## Parameters

- **Diameter** - The width across the sphere (default: 20mm)
- **Sides** - Number of segments around the perimeter (default: 40). More sides = smoother surface

### Advanced Parameters

Enable **Advanced** mode for additional controls:

- **Starting Angle** - Angle where the sphere surface begins (default: 0)
- **Ending Angle** - Angle where the sphere surface ends (default: 360). Set less than 360 for partial sphere shapes
- **Latitude Sides** - Number of segments from top to bottom (default: 30). More = smoother poles

## Tips

- For 3D printing, 40 sides is usually sufficient. Higher values create smoother surfaces but larger files
- Use Starting and Ending Angles to create partial sphere shapes like bowls or domes
- Combine with [Subtract](../operations/boolean/subtract.md) to create spherical cavities

## Related

- [Half Sphere](half-sphere.md) - Just the top hemisphere
- [Torus](torus.md) - A donut shape
