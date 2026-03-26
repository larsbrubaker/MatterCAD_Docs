---
title: Editing Objects
parent: "Getting Started"
nav_order: 3
---
# Editing Objects

MatterCAD provides intuitive controls built right into the 3D view for moving, rotating, and scaling your objects. You can also edit object parameters in the Properties panel.

## Moving Parts


- **Drag on the bed** - Click and drag any object to slide it around on the workspace surface
- **Move up and down** - Use the vertical arrow control at the top of a selected object to adjust its height (Z position)
- For precise positioning, use the [Translate](../operations/transform/translate.md) operation or type exact values in the Properties panel

## Rotating Parts

![20260324 080843 paste 20260324 080843](https://matterhackers.github.io/MatterCAD_Docs/assets/20260324-080843-paste-20260324-080843.jpg)

Click on any of the **rotate corner controls** that appear when you select an object. These let you rotate the object on the plane of that control.

- Move your mouse over one of the angle indicators to snap the rotation to **45-degree increments**
- For precise rotation, use the [Rotate](../operations/transform/rotate.md) operation and enter an exact angle

## Scaling Parts

![20260324 080819 paste 20260324 080819](https://matterhackers.github.io/MatterCAD_Docs/assets/20260324-080819-paste-20260324-080819.jpg)


Click on any of the **scale corner controls** to resize your part on the workspace.

- Drag a corner to scale proportionally
- For precise sizing or non-uniform scaling, use the [Scale](../operations/transform/scale.md) operation where you can set exact dimensions or scale each axis independently

## Editing Parameters

When you select an object, its parameters appear in the Properties panel on the right side of the screen. For example:

- A **Cube** shows Width, Depth, Height, and optional Rounding controls
- A **Cylinder** shows Diameter, Height, and Sides
- A **Text** object shows the text content, font, size, and height

You can type values directly, use sliders, or enter [expressions](../workspace/expressions.md) for parametric relationships.

## Context Menu

Right-click on any object to access additional options including:

- Copy, Cut, Delete
- Group / Ungroup
- Available operations for the selected object
- Help for the specific object type (when available)

## Tips

- Hold **Shift** while clicking to select multiple objects, then move or operate on them together
- Press **Ctrl+Z** to undo any change you make
- Use [Align](../operations/placement/align.md) to precisely position multiple objects relative to each other
- Press **Space** to clear your selection

## Related

- [Viewport Navigation](viewport-navigation.md) - How to rotate, pan, and zoom the view
- [Selection](../workspace/selection.md) - Detailed selection behavior
- [Transform Operations](../operations/transform/index.md) - Precise transform controls
- [Keyboard Shortcuts](../workspace/keyboard-shortcuts.md) - All available shortcuts
