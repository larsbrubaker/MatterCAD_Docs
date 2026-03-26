---
title: Cylinder
parent: "Primitives"
nav_order: 5
---
# Cylinder

A round column shape with configurable diameter, height, and number of sides. The Cylinder is essential for creating pins, rods, holes, and round features.

<!--  Screenshot of a Cylinder primitive on the workspace -->
![20260318 183248 paste 20260318 183248](https://matterhackers.github.io/MatterCAD_Docs/assets/20260318-183248-paste-20260318-183248.jpg)


## Parameters

- **Diameter** - The width across the cylinder (default: 20mm)
- **Height** - How tall the cylinder is (default: 20mm)
- **Sides** - Number of segments around the perimeter (default: 40). Lower values create polygonal shapes (e.g., 6 for a hexagon)

### Advanced Parameters

Enable **Advanced** mode to access additional controls:

- **Diameter Top** - Set a different diameter for the top of the cylinder to create tapered or truncated cone shapes (default: matches Diameter)
- **Starting Angle** - Angle where the cylinder begins (default: 0). Use with Ending Angle to create partial cylinders
- **Ending Angle** - Angle where the cylinder ends (default: 360). Set less than 360 for pie-slice shapes

## Tips

- Set Sides to a low number to create regular polygons -- 6 for hexagons, 8 for octagons, etc.
- Use different Diameter and Diameter Top values to create truncated cones and tapered shapes
- Set Starting and Ending Angles to create pie-slice or arc shapes
- Cylinders make excellent cutting tools for creating round holes with [Subtract](../operations/boolean/subtract.md)

## Related

- [Cone](cone.md) - A cylinder that tapers to a point
- [Half Cylinder](half-cylinder.md) - A cylinder cut in half lengthwise
- [Ring](ring.md) - A hollow cylinder (tube)
