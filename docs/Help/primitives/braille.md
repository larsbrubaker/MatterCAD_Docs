---
title: Braille
parent: "Primitives"
nav_order: 2
---
# Braille

Generate 3D-printable Braille text from standard English text. The Braille tool supports both Grade 1 (letter-by-letter) and Grade 2 (contracted) Braille encoding.

<!-- Screenshot of a Braille object showing raised dots on the workspace -->
![20260318 182800 paste 20260318 182800](https://matterhackers.github.io/MatterCAD_Docs/assets/20260318-182800-paste-20260318-182800.jpg)


## How to Use

1. Add a **Braille** primitive from the Primitives panel
2. Type your text in the **Text to Encode** field
3. The tool automatically converts it to the correct Braille dot pattern

## Parameters

- **Text to Encode** - The English text to convert to Braille
- **Scale** - Adjust the overall size of the Braille output
- **Height** - The height of the raised Braille dots

## Tips

- Grade 2 Braille uses contractions and abbreviations for common words and letter combinations, making it more compact
- Standard Braille cell dimensions are used to ensure the output is readable
- Combine with a flat [Cube](cube.md) base to create a complete Braille label or sign
- For Braille cards with an integrated base, see [Braille Card](braille-card.md)

## Related

- [Braille Card](braille-card.md) - Braille with an integrated card base
- [Text](text.md) - Standard 3D text
