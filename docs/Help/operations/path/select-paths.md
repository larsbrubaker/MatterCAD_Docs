---
title: Select Paths
parent: "Path Operations"
grand_parent: "Operations"
nav_order: 7
---
# Select Paths

Select Paths lets you choose specific paths from a complex multi-path object. This is useful when you import an SVG or create text that contains multiple separate path elements and you only want to work with some of them.

<!-- IMAGE_NEEDED: Screenshot showing a multi-path object with specific paths selected -->

## How to Use

1. Select an object that contains multiple paths (like an SVG import or text object)
2. Apply **Select Paths** from the Path operations menu
3. Choose which paths to include or exclude

## Tips

- Use this to isolate specific letters from a text object
- Useful for working with complex SVG files that contain many separate shapes
- After selecting, apply [Linear Extrude](linear-extrude.md) or other operations to only the selected paths

## Related

- [Merge Path](merge-path.md) - Combine multiple paths into one
- [SVG Object](../../primitives/svg-object.md) - Import SVGs that may need path selection
- [Text](../../primitives/text.md) - Text objects contain per-letter paths
