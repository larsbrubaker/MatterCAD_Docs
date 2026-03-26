---
title: Cone
parent: "Primitives"
nav_order: 3
---
# Cone

A tapered cylinder that comes to a point at the top. Useful for creating pointed features, funnels, and chamfers.

<!--  Screenshot of a Cone primitive on the workspace -->
![20260318 183159 paste 20260318 183159](https://matterhackers.github.io/MatterCAD_Docs/assets/20260318-183159-paste-20260318-183159.jpg)


## Parameters

- **Diameter** - The width across the base (default: 20mm)
- **Height** - How tall the cone is (default: 20mm)
- **Sides** - Number of segments around the perimeter (default: 40)

## Tips

- For a truncated cone (flat top instead of a point), use a [Cylinder](cylinder.md) with Advanced mode and set different Diameter and Diameter Top values
- Cones are useful for creating chamfered edges when combined with [Subtract](../operations/boolean/subtract.md)

## Related

- [Cylinder](cylinder.md) - A round column without taper
- [Pyramid](pyramid.md) - A four-sided pointed shape
