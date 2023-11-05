# History

## Is static
Derives from object

## Summary

Undo/redo history for the current active mapdoc
## Methods

```c#
static void Keep( MapNode node) 
```
Keeps a map node and all its children, so changes to it can be undone.
```c#
static void KeepNew( MapNode node) 
```
Keeps a new object node and all of its children, so they can be deleted on an undo.
```c#
static void MarkUndoPosition( string name) 
```
Mark new undo position
