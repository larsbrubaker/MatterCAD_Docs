---
title: Expressions
parent: "Workspace"
nav_order: 2
---
# Expressions

Many parameters in MatterCAD accept mathematical expressions instead of plain numbers. This enables parametric design where changing one value automatically updates related dimensions.

<!--  Screenshot showing an expression being entered in a parameter field -->
![20260318 193631 paste 20260318 193631](https://matterhackers.github.io/MatterCAD_Docs/assets/20260318-193631-paste-20260318-193631.jpg)


## How to Use

Instead of typing a plain number in a parameter field, you can type a math expression. For example:

- `20 + 5` evaluates to 25
- `pi * 10` evaluates to 31.416
- `width * 2` references another parameter named "width"

## Available Constants

- **pi** - 3.14159... (the ratio of circumference to diameter)
- **tau** - 6.28318... (2 * pi, a full revolution in radians)

## Supported Operations

- Addition: `+`
- Subtraction: `-`
- Multiplication: `*`
- Division: `/`
- Parentheses: `(` and `)` for grouping

## Tips

- Expressions are supported in any field that shows `DoubleOrExpression`, `IntOrExpression`, or `StringOrExpression` in the code -- in practice, most numeric fields in design tools accept them
- Use expressions to create relationships between parameters -- for example, set a hole's diameter to `outer_diameter - 4` so it always has 2mm walls
- Expressions update automatically when referenced values change
- You can use expressions in [Array](../operations/array/index.md) operations to create parametric patterns

## Related

- [Components](components.md) - Create reusable parameterized designs
- [Editing Objects](../getting-started/editing-objects.md) - Working with object parameters
