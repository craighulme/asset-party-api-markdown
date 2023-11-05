# MapNode

## ```c#
Implements IHandle
```

## Summary

A common class used for all objects in the world object tree.
## Properties

```c#
Angles Angles { get; set; } 
```
Euler angles of this map node.
```c#
IEnumerable<MapNode> Children { get; } 
```
Each MapNode can have many children. Children usually transform with their parents, etc.
```c#
string Name { get; set; } 
```
User specified name of this node
```c#
MapNode Parent { get; set; } 
```
The parent node, at the top level this will be theMapDoc.MapWorld
```c#
Vector3 Position { get; set; } 
```
World position of this map node.
```c#
Vector3 Scale { get; set; } 
```
Non-uniform scalar for this map node.
```c#
string TypeString { get; } 
```
Native C++ type name for this map node (nice for debug, might disappear at some point)
```c#
bool Visible { get; set; } 
```
Visibility of this MapNode, e.g if it's been hidden by the user
## Methods

```c#
MapNode Copy( ) 
```
Creates a copy of this map node.
```c#
override string ToString( ) 
```
OverridesObject.ToStringMap node types implement this to describe themselves and their children.
e.g CMapEntity returns "Entity: entity_name" or CMapMesh returns "Mesh (2 faces)"
## Inheriting Types

