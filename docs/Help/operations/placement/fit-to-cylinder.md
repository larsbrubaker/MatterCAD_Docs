---
title: Fit to Cylinder
parent: "Placement Operations"
grand_parent: "Operations"
nav_order: 3
---
# Fit to Cylinder

Fit to Cylinder scales and positions an object to fit within a cylindrical volume with a specified diameter and height.

<!-- IMAGE_NEEDED: Screenshot showing an object fit within a cylindrical boundary -->

## How to Use

1. Select an object
2. Apply the **Fit to Cylinder** operation from the Placement menu
3. Set the target cylinder dimensions

## Parameters

- **Diameter** - The diameter of the target cylinder
- **Height** - The height of the target cylinder
- **Stretch Z** - Enable or disable scaling along the Z axis to fit the cylinder height (default: on)
- **Alternate Centering** - When off, the object is expanded to fill the cylinder. When on, the visual weight of the object is centered within the cylinder, which works better for irregular shapes.

## Tips

- Use this when you need an object to fit within a round boundary, such as embedding a design in a cylindrical case
- Alternate Centering is useful for organic or asymmetric shapes where simple expansion would look off-center

## Related

- [Fit to Bounds](fit-to-bounds.md) - Fit within a rectangular boundary
- [Scale](../transform/scale.md) - Manual scaling
- [Align](align.md) - Position objects relative to each other
