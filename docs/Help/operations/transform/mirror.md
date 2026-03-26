---
title: Mirror
parent: "Transform Operations"
grand_parent: "Operations"
nav_order: 1
---
# Mirror

Mirror creates a reflected copy of an object across one of the three primary axes. The result is a mirrored version of the original shape.

<!-- IMAGE_NEEDED: Before and after showing an object mirrored across the X axis -->

## How to Use

1. Select an object
2. Apply the **Mirror** operation from the Transform menu
3. Choose which axis to mirror across

## Parameters

- **Mirror On** - The axis to mirror across:
  - **X Axis** - Flips the object left to right
  - **Y Axis** - Flips the object front to back
  - **Z Axis** - Flips the object top to bottom

## Tips

- Mirror is centered on the object's bounding box, so the mirrored result occupies the same space as the original
- Face normals are automatically corrected after mirroring to maintain proper rendering
- Use Mirror to create symmetrical designs -- model one half, then mirror it and [Combine](../boolean/combine.md) with the original
- Mirror is non-destructive: you can change the mirror axis at any time

## Related

- [Rotate](rotate.md) - Rotate an object instead of mirroring
- [Scale](scale.md) - Resize an object
- [Combine](../boolean/combine.md) - Merge the original and mirrored copy into one object
