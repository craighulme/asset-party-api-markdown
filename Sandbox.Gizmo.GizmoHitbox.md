# GizmoHitbox

## 
```c#
Derives from object
```

## Summary

Contains functions to add objects to the immediate mode Scene. This
is an instantiable class so it's possible to add extensions.
## Properties

```c#
bool Debug { get; } 
```
No Summary
```c#
float DepthBias { get; set; } 
```
No Summary
## Methods

```c#
void AddPotentialLine( in Vector3 p0, in Vector3 p1, float thickness) 
```
If we're in a hitbox linescope we'll distance this test vs the current ray. If
not, we'll return immediately.
This is automatically called when rendering lines
```c#
void BBox( BBox bounds) 
```
A bounding box hitbox
```c#
void Circle( Vector3 center, Vector3 forward, float outerRadius, float innerRadius = 0) 
```
A 2d circle hitbox, on a plane
```c#
IDisposable LineScope( ) 
```
Start a line scope. Any drawn lines should become a hitbox during this scope.
```c#
void Model( Model model, float maxDistance = 10000) 
```
A bounding box hitbox
```c#
void Sphere( Sphere sphere) 
```
A sphere hitbox
```c#
void TrySetHovered( float distance) 
```
If this distance is closer than our previous best, this path will become the hovered path
```c#
void TrySetHovered( Vector3 position) 
```
If this distance is closer than our previous best, this path will become the hovered path
