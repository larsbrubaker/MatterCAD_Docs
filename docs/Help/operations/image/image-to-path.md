---
title: Image to Path
parent: "Image Operations"
grand_parent: "Operations"
nav_order: 2
---
# Image to Path

Image to Path traces the outlines of an image to create 2D paths. These paths can then be extruded, revolved, or used with any other path operation. This is ideal for converting logos, silhouettes, and simple graphics into 3D objects.

![20260324 075521 paste 20260324 075521](https://matterhackers.github.io/MatterCAD_Docs/assets/20260324-075521-paste-20260324-075521.jpg)


## How to Use

1. Select an image object in your workspace
2. Apply **Image to Path** from the Image operations menu
3. Choose the analysis type and adjust the selection range

## Parameters

- **Analysis Type** - How the image is analyzed for tracing:
  - **Transparency** - Trace based on transparent vs opaque areas (best for PNGs with transparent backgrounds)
  - **Colors** - Trace based on color regions
  - **Intensity** - Trace based on brightness levels (best for most images)
- **Select Range** - A histogram control to select which brightness/color values to include in the trace
- **Min Surface Area** - Minimum area for a path loop to be included. Increase to filter out small noise artifacts

## Tips

- Clean, high-contrast images with simple shapes work best
- Use Transparency mode for PNG images with transparent backgrounds
- Use Intensity mode for photographs and images without transparency
- After tracing, apply [Linear Extrude](../path/linear-extrude.md) to give the path height
- Increase Min Surface Area to remove small unwanted details from the trace

## Related

- [Image Converter](image-converter.md) - Create height-map relief instead of flat paths
- [Lithophane](lithophane.md) - Create backlit image displays
- [SVG Object](../../primitives/svg-object.md) - Import vector graphics directly (no tracing needed)
- [Linear Extrude](../path/linear-extrude.md) - Give the traced path height
