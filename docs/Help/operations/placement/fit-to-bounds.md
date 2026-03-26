---
title: Fit to Bounds
parent: "Placement Operations"
grand_parent: "Operations"
nav_order: 2
---
# Fit to Bounds

Fit to Bounds scales an object to fit within specified width, depth, and height dimensions. You can control how the object stretches and aligns within the target bounds.

<!-- IMAGE_NEEDED: Screenshot showing an object being fit to specific bounding dimensions -->

## How to Use

1. Select an object
2. Apply the **Fit to Bounds** operation from the Placement menu
3. Enter the target dimensions
4. Choose proportion locking and stretch behavior

## Parameters

- **Lock Proportion** - How to constrain proportions:
  - **None** - Each axis can be set independently
  - **X & Y** - Width and depth are locked together
  - **X, Y & Z** - Uniform scaling on all axes
- **Width** - Target width (X dimension)
- **Depth** - Target depth (Y dimension)
- **Height** - Target height (Z dimension)

### When Lock Proportion is X & Y or X, Y & Z

- **Stretch** - How the object fits:
  - **Inside** - Scale down to fit entirely within the bounds (may leave gaps)
  - **Expand** - Scale up to fill the bounds (may exceed in some dimensions)

### When Lock Proportion is None

Each axis has its own:

- **Stretch** - Inside or Expand per axis
- **Align** - Where to position within the bounds (Min, Center, Max)

## Tips

- Use this to resize imported models to exact target dimensions
- Lock all proportions for uniform scaling that maintains the original shape
- Use per-axis control when you need to fit a specific width but don't care about the other dimensions

## Related

- [Scale](../transform/scale.md) - Scale by ratio or percentage instead of target size
- [Fit to Cylinder](fit-to-cylinder.md) - Fit within a cylindrical boundary
- [Align](align.md) - Position objects relative to each other
