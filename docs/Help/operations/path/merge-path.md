---
title: Merge Path
parent: "Path Operations"
grand_parent: "Operations"
nav_order: 4
---
# Merge Path

Merge Path combines multiple separate paths into a single unified path. This is the path equivalent of [Combine](../boolean/combine.md) for 3D objects.

<!-- IMAGE_NEEDED: Before and after showing separate paths merged into one -->

## How to Use

1. Select an object containing multiple paths
2. Apply **Merge Path** from the Path operations menu
3. The separate paths are merged into a single path

## Tips

- Use this before [Linear Extrude](linear-extrude.md) when you want multiple paths to be treated as one shape
- Merging overlapping paths creates a union of their areas

## Related

- [Select Paths](select-paths.md) - Select specific paths from a group
- [Combine](../boolean/combine.md) - The 3D equivalent for merging solid objects
- [Linear Extrude](linear-extrude.md) - Give the merged path height
