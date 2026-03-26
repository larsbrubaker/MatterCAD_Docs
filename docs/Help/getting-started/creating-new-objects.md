---
title: Creating New Objects
parent: "Getting Started"
nav_order: 2
---
# Creating New Objects

MatterCAD provides a rich set of tools for creating 3D objects. You can start with primitive shapes, use specialized tools like text and QR codes, or build complex forms using boolean operations and arrays.

![20260324 081122 paste 20260324 081122](https://matterhackers.github.io/MatterCAD_Docs/assets/20260324-081122-paste-20260324-081122.jpg)

## Adding Primitives

The fastest way to start a design is by adding primitive shapes. Open the Primitives panel in the library and click on any shape to add it to your workspace. Available primitives include:

- **Basic shapes** - Cube, Cylinder, Sphere, Cone, Torus, Ring, Pyramid, Wedge, and their half variants
- **Text and special** - Text, Braille, QR Code, Image Object, SVG Object

Each primitive has parameters you can adjust in the Properties panel after selecting it. For example, a Cube has Width, Depth, and Height controls. See [Primitives](../primitives/index.md) for details on each shape.

## The Operations Toolbar

![20260324 081005 paste 20260324 081005](https://matterhackers.github.io/MatterCAD_Docs/assets/20260324-081005-paste-20260324-081005.jpg)

The toolbar at the top of the viewport gives you quick access to common operations:

- **Undo / Redo** - Reverse or replay changes. You can also use **Ctrl+Z** to undo and **Ctrl+Y** to redo
- **Group / Ungroup** - Combine selected objects into a group that moves and operates as one unit, or break a group apart
- **Copy / Delete** - Duplicate or remove selected objects. Standard **Ctrl+C**, **Ctrl+X**, and **Ctrl+V** shortcuts also work
- **Align** - Position multiple objects relative to each other
- **Boolean operations** - [Combine](../operations/boolean/combine.md), [Subtract](../operations/boolean/subtract.md), [Intersect](../operations/boolean/intersect.md), and [Subtract & Replace](../operations/boolean/subtract-and-replace.md)
- **Arrays** - Create [Linear](../operations/array/linear-array.md), [Radial](../operations/array/radial-array.md), or [Advanced](../operations/array/advanced-array.md) patterns of duplicated objects
- **Transforms** - Apply [Rotate](../operations/transform/rotate.md), [Scale](../operations/transform/scale.md), [Mirror](../operations/transform/mirror.md), and other modifications

## Building Complex Shapes

Most designs in MatterCAD are built by combining simple shapes:

1. **Start with primitives** - Add the basic shapes you need
2. **Position them** - Move and rotate objects so they overlap where you want
3. **Apply boolean operations** - Use [Combine](../operations/boolean/combine.md) to merge shapes together, or [Subtract](../operations/boolean/subtract.md) to cut one shape out of another
4. **Refine** - Use [Reshape](../operations/reshape/index.md) operations like Bevel, Curve, or Twist to add detail

## Related

- [Primitives](../primitives/index.md) - Full reference for all primitive shapes
- [Adding Existing Objects](adding-existing-objects.md) - Import files instead of creating from scratch
- [Boolean Operations](../operations/boolean/index.md) - Combine shapes into complex forms
- [Editing Objects](editing-objects.md) - Move, rotate, and scale objects after creating them
