---
title: Image Converter
parent: "Image Operations"
grand_parent: "Operations"
nav_order: 1
---
# Image Converter

Image Converter turns a raster image into a 3D relief where pixel brightness determines height. Bright areas become raised and dark areas become low (or vice versa).

![20260323 210414 paste 20260323 210414](https://matterhackers.github.io/MatterCAD_Docs/assets/20260323-210414-paste-20260323-210414.jpg)


## How to Use

1. Add an Image Converter from the Primitives panel, or drag an image file onto the workspace
2. The image is converted to a 3D height map
3. Adjust the height and other parameters

## Tips

- High-contrast images with clear shapes produce the best results
- For tracing image outlines as flat paths instead of height maps, use [Image to Path](image-to-path.md)
- For creating backlit image displays, use [Lithophane](lithophane.md)
- You can drag images directly from your desktop onto the workspace
- Add a base by combining the image relief with a [Cube](../../primitives/cube.md)

## Related

- [Image to Path](image-to-path.md) - Trace outlines instead of creating a height map
- [Lithophane](lithophane.md) - Create backlit image displays
- [Image Object](../../primitives/image-object.md) - The primitive version of image import
