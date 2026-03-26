---
title: Adding Existing Objects
parent: "Getting Started"
nav_order: 1
---
# Adding Existing Objects

You can bring existing 3D models into MatterCAD by importing files from your computer or adding content from the built-in library.

## From Your Computer

![20260324 081143 paste 20260324 081143](https://matterhackers.github.io/MatterCAD_Docs/assets/20260324-081143-paste-20260324-081143.jpg)

![20260324 081240 paste 20260324 081240](https://matterhackers.github.io/MatterCAD_Docs/assets/20260324-081240-paste-20260324-081240.jpg)


Click the **Open** button in the toolbar to browse and add files from your computer. MatterCAD supports the following import formats:

- **STL** (.stl) - Industry standard 3D model format, widely used for 3D printing
- **AMF** (.amf) - Advanced format supporting colors and multi-material objects
- **OBJ** (.obj) - Wavefront 3D graphics format (mesh geometry only)
- **3MF** (.3mf) - 3D Manufacturing Format with rich metadata support
- **MCX** (.mcx) - MatterCAD's native format, preserving all design data and parameters
- **SVG** (.svg) - Scalable Vector Graphics, imported as 2D paths
- **TTF / OTF** (.ttf, .otf) - Font files for use with the Text tool

## Drag and Drop

You can also drag and drop files directly from your desktop or file explorer into the MatterCAD workspace. Supported file types will be imported automatically.

![20260324 081416 paste 20260324 081416](https://matterhackers.github.io/MatterCAD_Docs/assets/20260324-081416-paste-20260324-081416.jpg)

## From the Library

### The Library Sidebar

Click the **Add Content** button in the toolbar to open the library browser panel. From here you can:

- Browse your saved designs
- Navigate to the Primitives library for built-in shapes
- Access your Cloud Library if signed in
- Drag and drop any item from the library directly into your workspace

![20260324 081446 paste 20260324 081446](https://matterhackers.github.io/MatterCAD_Docs/assets/20260324-081446-paste-20260324-081446.jpg)

### The Library Tab

You can also use the Library tab to browse your collections. Right-click on any object in the library and select **Add to Scene** to import it into your current design workspace.

![20260324 081536 paste 20260324 081536](https://matterhackers.github.io/MatterCAD_Docs/assets/20260324-081536-paste-20260324-081536.jpg)

## Tips

- MCX is the best format for re-editing designs later, since it preserves all parameters and the design tree
- STL files contain only mesh geometry. If you import an STL, you can still apply operations to it, but you cannot edit the original parameters
- When importing multiple files, each one becomes a separate object in your scene. Use [Group](../workspace/grouping.md) to organize them

## Related

- [Creating New Objects](creating-new-objects.md) - Start a design from scratch with primitives
- [Saving and Exporting](saving-and-exporting.md) - Save and export your finished designs
- [Library](../library/index.md) - Learn more about organizing your design library
