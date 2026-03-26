---
title: Repair
parent: "Mesh Operations"
grand_parent: "Operations"
nav_order: 2
---
# Repair

Repair fixes common problems in mesh geometry, including non-manifold edges, holes, inconsistent face orientation, and nearly-coincident vertices. This is especially useful for imported STL and OBJ files that may have errors.

![20260324 080517 paste 20260324 080517](https://matterhackers.github.io/MatterCAD_Docs/assets/20260324-080517-paste-20260324-080517.jpg)


## How to Use

1. Select an object with mesh problems
2. Apply the **Repair** operation from the Mesh menu
3. Review the before/after statistics to see what was fixed

## Statistics (Read Only)

- **Initial Vertices / Final Vertices** - Vertex count before and after repair
- **Initial Faces / Final Faces** - Face count before and after repair
- **Initial Non-Manifold Edges / Final Non-Manifold Edges** - Problem edge count before and after

### Advanced Options

Enable **Advanced** mode for fine-grained control:

- **Weld Vertices** - Merge nearly-coincident vertices (default: on)
- **Weld Tolerance** - How close vertices must be to merge
- **Face Orientation** - Make all faces consistently oriented
- **Weld Edges** - Repair small cracks and bad seams
- **Fill Holes** - Fill gaps in the mesh surface
- **Remove Mode** - Remove internal or occluded geometry:
  - **None** - Keep all geometry
  - **Interior** - Remove internal bodies hidden inside the main shape
  - **Occluded** - Remove faces blocked from outside view

## Tips

- Try Repair first if boolean operations (Combine, Subtract) produce unexpected results on imported models
- The default settings (Weld Vertices on, everything else off) fix the most common issues
- Enable Fill Holes if you can see through gaps in the model
- Use Remove Interior to clean up models that have hidden geometry inside

## Related

- [Decimate](decimate.md) - Reduce polygon count
- [Adding Existing Objects](../../getting-started/adding-existing-objects.md) - Import models that may need repair
