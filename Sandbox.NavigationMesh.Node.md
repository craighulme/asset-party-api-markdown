# Node

## 
```c#
Derives from object
```

## Summary

Connections from this area to other areas
## Fields

```c#
List<Connection> Connections
```
Connections from this area to other areas
## Properties

```c#
BBox BoundingBox { get; } 
```
No Summary
```c#
Vector3 Center { get; } 
```
No Summary
```c#
Vector3 Normal { get; } 
```
No Summary
```c#
IEnumerable<Triangle> Triangles { get; } 
```
Iterate the triangles of this node. This will be 1 or 2 triangles.
```c#
List<Vector3> Vertices { get; } 
```
No Summary
## Methods

```c#
Vector3 ClosestPoint( Vector3 point) 
```
Find the closest point on this area
```c#
float Distance( Vector3 point) 
```
Get the distance away from this point
## Nested Types

