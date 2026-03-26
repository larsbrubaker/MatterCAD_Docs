---
title: Undo and Redo
parent: "Workspace"
nav_order: 9
---
# Undo and Redo

MatterCAD maintains a full history of your changes so you can undo mistakes and redo actions you reversed.

## How to Use

- **Ctrl + Z** - Undo the last action
- **Ctrl + Y** or **Ctrl + Shift + Z** - Redo the last undone action
- You can also use the **Undo** and **Redo** buttons in the toolbar

## What Can Be Undone

All design operations are tracked in the undo history, including:

- Adding or deleting objects
- Moving, rotating, and scaling objects
- Applying operations (boolean, transform, reshape, etc.)
- Changing object parameters
- Grouping and ungrouping

## Tips

- You can undo multiple steps by pressing Ctrl + Z repeatedly
- The undo history is maintained for the current session. Closing and reopening a design starts a fresh history.
- If you undo several steps and then make a new change, the redo history beyond that point is cleared

## Related

- [Keyboard Shortcuts](keyboard-shortcuts.md) - All available shortcuts
- [Editing Objects](../getting-started/editing-objects.md) - Working with objects in the viewport
