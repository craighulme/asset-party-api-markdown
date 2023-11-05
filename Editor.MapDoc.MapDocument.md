# MapDocument

## ```c#
Implements IHandle
```

## Summary

Represents an open map document. A document has a tree ofMapDoc.MapNodethat represent the world.
## Properties

```c#
string PathName { get; } 
```
The map file name
```c#
MapWorld World { get; } 
```
The world
## Methods

```c#
void DeleteNode( MapNode node) 
```
Removes the node from the world, deletes all children too.
