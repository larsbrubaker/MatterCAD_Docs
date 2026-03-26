---
title: QR Code
parent: "Primitives"
nav_order: 12
---
# QR Code

Generate QR codes as 3D objects. You can encode text, URLs, or WiFi credentials into a scannable 3D QR code.

<!--  Screenshot of a 3D QR Code object on the workspace -->
![20260318 184540 paste 20260318 184540](https://matterhackers.github.io/MatterCAD_Docs/assets/20260318-184540-paste-20260318-184540.jpg)


## How to Use

1. Add a **QR Code** from the Primitives panel
2. Choose the output type (Text or WiFi)
3. Enter your content
4. The QR code is generated as a 3D object you can place on your design

## Parameters

### Text Mode

- **Text** - The text or URL to encode (default: "https://matterhackers.com")

### WiFi Mode

- **SSID** - The name of the WiFi network
- **Password** - The WiFi password
- **Security** - The security type (WEP, WPA, or None)

## Tips

- Use [Subtract](../operations/boolean/subtract.md) to engrave the QR code into a surface, or place it on top of a [Cube](cube.md) base
- Test that your QR code scans correctly with a phone before printing
- WiFi QR codes let people connect to your network by scanning the code
- Make sure the QR code is large enough to be scannable when printed -- at least 20-25mm across

## Related

- [Text](text.md) - Standard 3D text
- [Image Object](image-object.md) - Convert images to 3D
