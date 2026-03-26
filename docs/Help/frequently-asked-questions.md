---
title: Frequently Asked Questions
nav_order: 101
---
# Why are my objects the wrong scale?
- STL files don't store unit information. MatterCAD expects STL dimensions in millimeters, while most CAD software exports in their native units (typically inches). This causes scaling discrepancies when importing designs.

- The best solution is to configure your design software to export STL files in millimeters. For example, in SolidWorks, use the Options button in the Save As dialog to set STL export parameters.

- Alternatively, you can rescale the part within MatterCAD. In 3D View, enter Edit mode and select SCALE from the right toolbar. Use the dropdown menu for common conversion factors or enter specific dimensions in the axis fields.

# How do I clear the application data?

- If reinstalling doesn't resolve an issue, you may need to delete MatterCAD's stored data. This data persists after uninstallation. To completely reset to default settings, remove the application folder. You can also temporarily rename the SQLite database file (MatterCAD.db) to test if settings are causing problems.
![20260318 194137 paste 20260318 194137](https://matterhackers.github.io/MatterCAD_Docs/assets/20260318-194137-paste-20260318-194137.jpg)

![20260318 194200 paste 20260318 194200](https://matterhackers.github.io/MatterCAD_Docs/assets/20260318-194200-paste-20260318-194200.jpg)

![20260318 194218 paste 20260318 194218](https://matterhackers.github.io/MatterCAD_Docs/assets/20260318-194218-paste-20260318-194218.jpg)


- Windows
  - User library and settings are stored in C:\Users\{user}\AppData\Local\MatterCAD.
