# Result

## 
```c#
Derives from ValueType
```

## Summary

The distance between start and end positions.
## Fields

```c#
VertexDetail Vertex0
```
No Summary
```c#
VertexDetail Vertex1
```
No Summary
```c#
VertexDetail Vertex2
```
No Summary
## Properties

```c#
float Distance { get; set; } 
```
The distance between start and end positions.
```c#
Vector3 EndPosition { get; set; } 
```
The end or hit position of the trace
```c#
float Fraction { get; set; } 
```
A fraction [0..1] of where the trace hit between the start and the original end positions
```c#
bool Hit { get; set; } 
```
No Summary
```c#
Vector3 HitNormal { get; set; } 
```
The hit surface normal (direction vector)
```c#
Vector3 HitPosition { get; set; } 
```
The hit position of the trace
```c#
int HitTriangle { get; set; } 
```
No Summary
```c#
Vector2 HitTriangleUv { get; set; } 
```
This is the Uv coordinate on the triangle hit. 'x' represents the distance between Vertex 0-1, 'y' represents the distance between Vertex 0-2.
```c#
Material Material { get; set; } 
```
No Summary
```c#
SceneObject SceneObject { get; set; } 
```
If we hit something associated with a sceneobject, this will be that object.
```c#
Vector3 StartPosition { get; set; } 
```
The start position of the trace
```c#
Transform Transform { get; set; } 
```
The transform of the hit object (if it has one)
```c#
Vector3 VertexInfluence { get; set; } 
```
Given the position on the triangle hit, this vector gives the influence of each vertex on that position.
So for example, if the Vector is [1,0,0] that means that the hit point is right on vertex 0. If it's [0.33, 0.33, 0.33] then it's
right in the middle of each vertex.
## Nested Types

## Referencing Members

```c#
Result = MeshTraceRequest.Run( ) 
```
