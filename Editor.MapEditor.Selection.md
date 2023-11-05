# Selection

## Is static
Derives from object

## Summary

Current selection set for the active map
## Remarks

## Properties

```c#
static IEnumerable<MapNode> All { get; } 
```
All the map nodes in the current selection set
```c#
static Vector3 PivotPosition { get; set; } 
```
The position of the selection's pivot
```c#
static SelectMode SelectMode { get; set; } 
```
The current selection mode e.g Meshes or Objects
## Methods

```c#
static void Add( MapNode node) 
```
Add the map node to the current set
```c#
static void Clear( ) 
```
Clear everything from the current selection set
```c#
static void InvertSelection( ) 
```
Invert the current selection
```c#
static void Remove( MapNode node) 
```
Remove this map node from the current set if it exists
```c#
static void SelectAll( ) 
```
Add all to the current selection
```c#
static void Set( MapNode node) 
```
Clear the current set, making the map node the only selected node
## Events

```c#
static OnChanged( ) 
```
Called when the selection in Hammer is changed
