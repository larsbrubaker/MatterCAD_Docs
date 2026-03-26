---
title: Scale
parent: "Transform Operations"
grand_parent: "Operations"
nav_order: 3
---
# Scale

Scale resizes an object with precise control over dimensions, proportions, and unit conversion. You can scale uniformly, lock specific axes together, or resize each axis independently.

<!-- IMAGE_NEEDED: Screenshot showing the Scale operation properties with dimension fields and lock proportion options -->

## How to Use

1. Select an object
2. Apply the **Scale** operation from the Transform menu
3. Choose your scaling method and enter the desired values

You can also scale objects in the viewport by clicking and dragging the scale corner controls on a selected object.

## Parameters

### Scale Type

Choose a preset or custom scaling:

- **Custom** - Enter your own dimensions or percentages
- **Inches to mm** - Multiply by 25.4 (convert imperial to metric)
- **mm to Inches** - Multiply by 0.0393 (convert metric to imperial)
- **mm to cm** - Multiply by 0.1
- **cm to mm** - Multiply by 10

### Scale Method (Custom mode)

- **Direct** - Enter the desired Width, Depth, and Height in millimeters
- **Percentage** - Enter Width, Depth, and Height as percentages of the original size

### Lock Proportion

- **None (Scale Freely)** - Each axis scales independently
- **X & Y** - Width and Depth are locked together; Height scales independently
- **X, Y & Z** - All three axes scale together uniformly

### Dimensions

- **Width** - Size along the X axis
- **Depth** - Size along the Y axis
- **Height** - Size along the Z axis

## Tips

- Use "Inches to mm" if you imported an STL file that was designed in inches and appears too small
- Lock Proportion to X, Y & Z for uniform scaling -- changing any one dimension updates them all
- The object's base position is maintained during scaling so it stays on the workspace surface
- You can type exact values for precise sizing, or use the sliders for quick adjustments

## Related

- [Translate](translate.md) - Move an object
- [Rotate](rotate.md) - Rotate an object
- [Fit to Bounds](../placement/fit-to-bounds.md) - Scale to fit within a specific size
