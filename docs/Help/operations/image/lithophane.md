---
title: Lithophane
parent: "Image Operations"
grand_parent: "Operations"
nav_order: 3
---
# Lithophane

A lithophane is a thin 3D panel where an image is encoded as varying thickness. When backlit, the thinner areas let more light through, revealing the image. This creates a beautiful way to display photographs and artwork.

![20260324 080310 paste 20260324 080310](https://matterhackers.github.io/MatterCAD_Docs/assets/20260324-080310-paste-20260324-080310.jpg)


## How to Use

1. Import an image or select an existing image object
2. Apply the **Lithophane** operation
3. Adjust the resolution and dimensions
4. Print the result in a light-colored material and place in front of a light source

## Parameters

- **Pixels Per mm** - Resolution of the lithophane (default: 1.5, range: 0.5-3). Higher values capture more detail but create larger files
- **Height** - Maximum thickness of the lithophane panel (default: 2.5mm, range: 0.5-3mm)
- **Width** - Total width of the lithophane in pixels (default: 150)
- **Invert** - Reverse the light/dark mapping (default: on). Usually kept on for correct display when backlit

## Tips

- Print in white or light-colored material for best results
- A height of 2-3mm works well for most lithophanes
- Higher Pixels Per mm captures more detail but increases print time and file size
- Mount the finished print in a frame with LED backlighting for best visibility
- Portrait photos with good contrast work particularly well

## Related

- [Image Converter](image-converter.md) - Create raised relief from images instead
- [Image to Path](image-to-path.md) - Trace image outlines as paths
