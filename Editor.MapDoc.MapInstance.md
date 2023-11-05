# MapInstance

## 
```c#
Derives from MapNode
```

## Summary

A map node which allows a target group and its children to be placed with a new position
and orientation in the world without creating a new copy.Multiple MapInstance classes may reference the same target allowing it to be placed in
multiple locations, but allowing any edits to be applied to all instances.
## Constructors

```c#
MapInstance( MapDocument mapDocument = null) 
```
No Summary
## Properties

```c#
MapNode Target { get; set; } 
```
The target map node this MapInstance references to copy.
