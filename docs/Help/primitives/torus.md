---
title: Torus
parent: "Primitives"
nav_order: 17
---
# Torus

A donut-shaped ring with independent control over the overall size and the thickness of the ring cross-section.

<!--  Screenshot of a Torus primitive on the workspace -->
![20260318 184240 paste 20260318 184240](https://matterhackers.github.io/MatterCAD_Docs/assets/20260318-184240-paste-20260318-184240.jpg)


## Parameters

- **Outer Diameter** - The overall width across the torus (default: 20mm)
- **Inner Diameter** - The diameter of the hole in the center (default: 10mm)
- **Sides** - Number of segments around the main ring (default: 40)

### Advanced Parameters

Enable **Advanced** mode for additional controls:

- **Starting Angle** - Angle where the torus begins (default: 0)
- **Ending Angle** - Angle where the torus ends (default: 360). Set less than 360 for an open ring or arc
- **Ring Sides** - Number of segments around the cross-section of the ring (default: 15). More = smoother tube profile
- **Ring Phase Angle** - Rotates the cross-section profile (default: 0)

## Tips

- The ring tube thickness is determined by the difference between Outer and Inner Diameter
- Use Starting and Ending Angles to create open ring segments, arcs, or C-shapes
- Useful for creating O-rings, handles, decorative rings, and pipe bends

## Related

- [Ring](ring.md) - A straight-walled hollow cylinder (tube)
- [Sphere](sphere.md) - A solid ball shape
- [Half Sphere](half-sphere.md) - A dome shape
