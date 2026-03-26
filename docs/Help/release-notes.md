---
title: Release Notes
nav_order: 104
---
# MatterCAD 2.2026.3 (March 12, 2026)
[Windows Download](https://mattercontrol.appspot.com/downloads/mattercad-windows/release)

## New Features

* **All-New Direct3D 11 Rendering Engine**
  * Complete migration from OpenGL to Direct3D 11 for dramatically better performance
  * FXAA anti-aliasing for crisp, clean edges
  * Dual depth peeling for correct order-independent transparency
  * Hardware-accelerated bed shadows
  * Improved object outlines and selection visuals
  * ![Screenshot of a design with one object set to 50% transparency, showing objects behind it](https://img.matterhackers.com/g/Z3M6Ly9taC1pcHMtcHJvZC9jbXMtcHJvZC80NGNmZGZlOC02NGI1LTRiZTEtYjE4Ni0wYTRhZjkxYWQxYzQ)

* **Object Transparency**
  * Set alpha/transparency on any individual object in the scene
  * Per-face color meshes support alpha without color damage
  * ![Show rotating a scene with multiple transparent objects and bed shadows](https://img.matterhackers.com/g/Z3M6Ly9taC1pcHMtcHJvZC9jbXMtcHJvZC9iNjNhOWMxNy00MzE0LTQ0ZmUtOGFjZS1kMWVlMTdkMzEzMDE)
  
* **Lock & Hide Objects**
  * Lock objects to prevent accidental selection or editing
  * Hide objects to reduce visual clutter while working on specific parts
  * Unhide All and Unlock All commands to quickly restore visibility
  * Locked and hidden objects are correctly excluded from ray-based selection
  * ![Show locking an object (clicking lock icon), then trying to select it, then using Unlock All](https://www.matterhackers.com/r/g4j2gw)

* **Improved Boolean Subtract**
  * Multi-subtract operations are significantly more reliable and accurate

## Improvements

* **File Handling**
  * Projects now save as 3MF by default instead of STL, preserving colors, materials, and design history
  * Enhanced drag-and-drop support for files and folders into the 3D view

* **Workflow**
  * Save As and Move dialogs remember your last folder location
  * Expression fields now support `pi`, `tau`, `e`, and `count`
  * Esc key performs undo in design editing contexts
  * 3D controls remain visible when mouse leaves the scene

* **Performance & Stability**
  * Fixed startup crashes and recursive load issues
  * Fixed lighting and mipmapping rendering bugs
  * Improved library tree view updates
  * Dynamic near/far plane calculations for better zoom behavior
  * Upgraded to .NET 10

---

# MatterCAD 2.2025.6 (June 20, 2025)
[Windows Download](https://mattercontrol.appspot.com/downloads/development/ag9zfm1hdHRlcmNvbnRyb2xyQQsSB1Byb2plY3QYgICI5uHFqwoMCxINUHVibGljUmVsZWFzZRiAgIjH1paxCAwLEgZVcGxvYWQYgICIj46vnwsM)

## New Features

* **SVG File Support**  
  * Full drag-and-drop support for SVG files
  * Direct conversion from SVG graphics to 3D objects
  * Seamless integration with existing CAD workflows

* **Advanced OBJ File Handling**  
  * Support for loading materials from ZIP archives
  * Enhanced OBJ file parsing and material handling
  * Better support for complex 3D models with multiple materials

* **Enhanced Tab Management System**
  * Cloud library tabs now persist correctly - your work stays exactly where you left it
  * Improved tab organization and navigation
  * Automatic restoration of open tabs between sessions

## User Experience Enhancements

* **Streamlined Interface**
  * Reorganized Recent menu for faster access
  * Better visual feedback during long operations
  * Improved application startup time and responsiveness

* **Reliability**
  * Fixed critical crashes in 3D scene interactions
  * Resolved memory management issues
  * Improved application stability across all platforms

---

# MatterCAD 2.21.5 (Feb 13, 2025)

[Windows Download](https://mattercontrol.appspot.com/downloads/development/ag9zfm1hdHRlcmNvbnRyb2xyQQsSB1Byb2plY3QYgICI5uHFqwoMCxINUHVibGljUmVsZWFzZRiAgIiHsuvhCgwLEgZVcGxvYWQYgICIh-O2lgsM)

# Existing Features

*The following features represent the foundation that MatterCAD builds upon from MatterControl's heritage:*

* Added Hollow Feature  
 ![Hollow Example](https://lh3.googleusercontent.com/-ImcYYK1I3P7tvxJXLRYDitBkc2xfXD0mElN3tiX8mZk1-Qe0Gxm5TtXXzC-Er756XajqOPpu7HFEuflNCnbZZqEzg=w220) ![Hollow Menu](https://lh3.googleusercontent.com/JiCUdiJx0eboPJk2cQH3dMOvlrFsFcz7OK-v9nG3G8ztDDHovXw--xaDsN8-HbFhFfAz5jSFKHUNQwnee5WXRNApH2M=w120)
* Added Polygon Reduce  
![Reduce Options](https://lh3.googleusercontent.com/h6opzhbdA352u9JFtIcqPnrnJC4JjcoVehdFstGZHe1gu7qiupQ8KAYrngTORjSyUerGlxhX48sGHLlwF2AoPjG0ifw=w220) ![Reduce Menu](https://lh3.googleusercontent.com/Pw2RYm45dFljKfmAq65378bpwULWxH857_Gz_SB95JLsmQYF3YmhOJ-XFEtWqWcFcK4weNLmz2hnVggk_85jWFDE=w120) 
* Added Mesh Repair  
 ![Repair Options](https://lh3.googleusercontent.com/C-fT1jQ-z1oOU1uBzWNLCN2IsAGOGAmJdhmUKqQLhC3p9_WdeKFDNKSoTGb4U8RRDdYk2ZRbWJ2FbjfNKzo6ii6v=w220) ![Repair Menu](https://lh3.googleusercontent.com/uQ8uaWvzremfTd7jkSu7OhKURHfvyEAFtbT1_KaTL1wgSrSUOjjQ0tm1a6uROpe6JZwC50HvdB4bJcGq8XqGAUMwmg=w120) 
* Put in fully automatic support (legacy support) as an opption in additon to new manual support option
* Added Support for gsSlicer (Experimental new slicing engine)
* Fixed bugs

## Changes

* Improved ungrouping of mesh (splitting into multiple meshes)
    * Discard degenerate faces
    * Discard microscopic discrete features

## Changes

* Added search bar for application
    * ![Search](https://lh3.googleusercontent.com/pAN6dqaGJJZs0cVZZDtkY40IlLXeoHNFmoovzivkGdhzCwN65wuqQdYvguoVo7SewCNl33mbLMd__OVw6BJhhV1n)
* Improved design tool bar
    * Added grouping to some items
    * Added dual align button
    * Added Arrange All button
* Nudge items on the bed with arrow keys
* Downloads folder is sorted by date

## Changes

* UI improvements
    * Faster updates in Cloud Library folders
    * Restore UI on re-open
    * Better Keyboard navigation support
* New error detection and warning system
    * More hardware errors handled
* Design tools improvements and optimizations
    * New Twist tools 
    * Improved Curve tool
    * Improved Align


## Changes

* Improved flatten
* Improved Undo support
* Improved design history

## Changes
* Versioning: Moving to a (version).(year).(month) version number. Easier to read and more informative.
* New State-of-the-art Subtract, Combine and Intersection (Window only)
* We now start up with a 'Feature Tour' to help new users find their way

## Changes
* Design Tools - The ability to 3D model with a complete set of modeling primitives
* Use a primitive to create your own customized supports
* Design Apps - Design Apps: sophisticated customizable designs
* 64-bit Processing