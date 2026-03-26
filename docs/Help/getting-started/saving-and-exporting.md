---
title: Saving and Exporting
parent: "Getting Started"
nav_order: 4
---
# Saving and Exporting

MatterCAD supports several file formats for saving and exporting your designs. The format you choose depends on how you plan to use the file.

## Save Formats

### MCX (Native Format)

MCX is MatterCAD's native file format and the best choice for designs you want to continue editing later. It preserves:

- The full design tree with all objects and their hierarchy
- All parameters and settings for each object
- Boolean operations, arrays, and other operations in editable form
- Component relationships

**Use MCX when:** You want to save your work and continue editing it later.

### STL

STL is the most widely used format for 3D printing. It contains only the final triangle mesh geometry without any design history or parameters.

**Use STL when:** You want to 3D print your design or share it with someone who does not use MatterCAD.

### OBJ

OBJ (Wavefront) is a common 3D format supported by most 3D software. Like STL, it contains mesh geometry only.

**Use OBJ when:** You need to open your design in other 3D software like Blender or a game engine.

### SVG

SVG export creates a 2D vector file from the top-down view of your design. This is useful for laser cutting or CNC routing.

**Use SVG when:** You need a 2D outline of your design for laser cutting or engraving.

## How to Save

![20260324 080726 paste 20260324 080726](https://matterhackers.github.io/MatterCAD_Docs/assets/20260324-080726-paste-20260324-080726.jpg)

1. Open the **brand menu** (the MatterCAD logo in the top-left corner)
2. Select **Save As** to choose a location and format
3. Select the file format from the format dropdown
4. Choose where to save the file and click **Save**

Your design is also saved automatically as you work, so you will not lose changes if you close the application.

## Tips

- Always save an MCX copy of your design before exporting to STL or OBJ, so you can make changes later
- When exporting STL, all objects in the scene are merged into a single mesh
- If you need to share a design with someone who uses MatterCAD, send the MCX file to preserve full editability
- You can also save designs to your [Cloud Library](../library/cloud-library.md) for access from any computer

## Related

- [Adding Existing Objects](adding-existing-objects.md) - Import files into MatterCAD
- [Library](../library/index.md) - Organize your saved designs
- [Cloud Library](../library/cloud-library.md) - Store designs in the cloud
