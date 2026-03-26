---
title: Text
parent: "Primitives"
nav_order: 16
---
# Text

Create 3D extruded text with customizable content, font, size, and height. Text objects are great for labels, signs, nameplates, and decorative lettering.

<!--  Screenshot of a 3D Text object on the workspace showing extruded letters -->
![20260318 184207 paste 20260318 184207](https://matterhackers.github.io/MatterCAD_Docs/assets/20260318-184207-paste-20260318-184207.jpg)


## How to Use

1. Add a **Text** primitive from the Primitives panel
2. Type your text in the **Name** field in the Properties panel
3. Adjust the font, size, and extrusion height as needed

## Parameters

- **Name** - The text content to display
- **Point Size** - The font size. This is accurate relative to standard print sizing -- a 12-point size in MatterCAD matches 12-point type on a 2D printer
- **Height** - The extrusion height (how far the text sticks up from the surface)
- **Font** - Select from available system fonts

## Tips

- Use [Subtract](../operations/boolean/subtract.md) to engrave text into a surface instead of raising it
- For very small text, increase the Point Size and then [Scale](../operations/transform/scale.md) down the entire object for better detail
- Each letter in the text is a separate path that gets extruded together

## Related

- [Braille](braille.md) - Generate 3D-printable Braille text
- [QR Code](qr-code.md) - Generate a QR code as a 3D object
- [Image Object](image-object.md) - Convert images to 3D
