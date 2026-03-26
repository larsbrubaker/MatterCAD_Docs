---
title: Linear Extrude
parent: "Path Operations"
grand_parent: "Operations"
nav_order: 3
---
# Linear Extrude

Linear Extrude gives a 2D path height, turning a flat shape into a 3D solid. This is the primary way to convert paths into 3D objects.

<!-- IMAGE_NEEDED: Before and after showing a 2D star path extruded into a 3D star -->

## How to Use

1. Select a 2D path or path-based object
2. Apply **Linear Extrude** from the Path operations menu
3. Set the desired height

## Parameters

- **Height** - How tall the extrusion is (default: 5mm, range: 0.1-50mm)
- **Bevel Top** - Add a beveled (rounded) edge to the top of the extrusion (default: off)

### Bevel Parameters (visible when Bevel Top is enabled)

- **Style** - The bevel profile style (Sharp or rounded)
- **Radius** - How wide the bevel extends (default: 3mm)
- **Segments** - Smoothness of the bevel curve (default: 9)

## Tips

- This works with any 2D path: [Circle](../../2d-paths/circle-path.md), [Box](../../2d-paths/box-path.md), [Star](../../2d-paths/star-path.md), [SVG](../../primitives/svg-object.md), and [Custom](../../2d-paths/custom-path.md) paths
- Enable Bevel Top for a more polished, professional look
- For revolving a path around an axis instead of extruding straight up, see [Revolve](revolve.md)

## Related

- [Revolve](revolve.md) - Spin a path around an axis
- [2D Paths](../../2d-paths/index.md) - Available path shapes
- [Text](../../primitives/text.md) - Text is automatically extruded
