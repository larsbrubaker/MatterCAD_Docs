---
title: Threads
parent: "Mechanical Parts"
nav_order: 3
---
# Threads

Create screw threads with configurable diameter, pitch, and thread profile. Threads can be used as standalone bolts/screws or subtracted from other objects to create threaded holes.

<!-- AUTO_IMAGE: type=from_thumbnail item=threads file=mechanical_threads -->
![mechanical_threads](https://matterhackers.github.io/MatterCAD_Docs/assets/mechanical_threads.png)

## How to Use

1. Add **Threads** from the Mechanical tools or Primitives panel
2. Set the diameter, pitch, and number of rotations
3. Optionally enable "Use as Hole" for creating threaded holes

## Parameters

### Usage

- **Use as Hole** - When enabled, the threads are sized with extra tolerance for use as a subtracted hole (default: off)
- **Tolerance** - Extra clearance for fit when used as a hole (default: 0.2mm, visible when Use as Hole is on)

### Attributes

- **Diameter** - The outer diameter of the threaded section (default: 10mm)
- **Pitch** - Distance between each thread turn (default: 2mm). Smaller pitch = finer threads
- **Thread Scale** - Width of the threads as a ratio of the pitch (default: 1.0, range: 0.1-1.0)
- **Rotations** - Number of complete thread turns (default: 10)

### Geometry

- **Sides** - Number of segments around the perimeter (default: 40). More = smoother

### Tips (Thread Ends)

- **Tip Scale** - How much to taper the thread ends (default: 0, range: 0-1). Set above 0 to create tapered lead-in at the ends
- **Tip Angle** - The angle over which to taper the tips (default: 90 degrees)

## Tips

- To create a threaded hole: enable "Use as Hole", position the threads, and [Subtract](../operations/boolean/subtract.md) from your object
- Add Tolerance when using as a hole to ensure the printed parts fit together
- Standard metric thread pitches: M3=0.5mm, M4=0.7mm, M5=0.8mm, M6=1.0mm, M8=1.25mm, M10=1.5mm
- Use Tip Scale to create a lead-in that makes it easier to start threading

## Related

- [Gears](gears.md) - Create mechanical gear shapes
- [Cylinder](../primitives/cylinder.md) - A plain round column (no threads)
- [Subtract](../operations/boolean/subtract.md) - Cut threads out of other objects to create holes
