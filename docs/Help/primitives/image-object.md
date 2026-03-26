---
title: Image Object
parent: "Primitives"
nav_order: 10
---
# Image Object

Import an image and convert it into a 3D relief object where brightness values determine the height of each pixel. This lets you turn photographs, logos, and artwork into 3D-printable objects.

<!-- Screenshot showing an image converted to a 3D relief on the workspace -->
![20260318 183708 paste 20260318 183708](https://matterhackers.github.io/MatterCAD_Docs/assets/20260318-183708-paste-20260318-183708.jpg)


## How to Use

1. Add an **Image Converter** from the Primitives panel, or drag an image file directly onto the workspace
2. Select or change the image using the properties
3. Adjust the height to control how much the bright areas are raised

## Parameters

- **Height** - How tall the raised portions of the image are
- The image preview shows in the Properties panel

## Tips

- High-contrast images with clear shapes work best
- You can drag images directly from your desktop onto the MatterCAD workspace
- Use the overflow menu tools on an imported image for more conversion options
- For path-based outlines from images, see [Image to Path](../operations/image/image-to-path.md)
- For backlit image displays, see [Lithophane](../operations/image/lithophane.md)
- Add a base by combining the image object with a [Cube](cube.md)

## Related

- [Image to Path](../operations/image/image-to-path.md) - Trace image outlines as 2D paths
- [Lithophane](../operations/image/lithophane.md) - Create images that appear when backlit
- [SVG Object](svg-object.md) - Import vector graphics
