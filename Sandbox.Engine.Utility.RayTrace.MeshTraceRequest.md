# MeshTraceRequest

## Derives from ValueType

## Summary

Casts a ray from point A to point B.
## Methods

```c#
MeshTraceRequest Ray( in Vector3 from, in Vector3 to) 
```
Casts a ray from point A to point B.
```c#
MeshTraceRequest Ray( in Ray ray, in float distance) 
```
Casts a ray from a given position and direction, up to a given distance.
```c#
Result Run( ) 
```
Run the trace and return the result. The result will return the first hit.
```c#
MeshTraceRequest WithAllTags( string[] tags) 
```
Only return scene objects with all of these tags
```c#
MeshTraceRequest WithAnyTags( string[] tags) 
```
Only return scene objects with any of these tags
```c#
MeshTraceRequest WithoutTags( string[] tags) 
```
Only return scene objects without any of these tags
```c#
MeshTraceRequest WithTag( string tag) 
```
Only return scene objects with this tag. Subsequent calls to this will add multiple requirements
and they'll all have to be met (ie, the scene object will need all tags).
## Nested Types

## Referencing Members

```c#
MeshTraceRequest = Model.Trace { get; } 
```
```c#
MeshTraceRequest = SceneWorld.Trace { get; } 
```
