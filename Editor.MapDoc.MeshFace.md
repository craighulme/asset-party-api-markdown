# MeshFace

## Derives from object

## Summary

Describes a face of aMapDoc.PolygonMesh.
## Constructors

```c#
MeshFace( Material material = null) 
```
No Summary
```c#
MeshFace( IEnumerable<int> indices, Material material = null) 
```
No Summary
## Properties

```c#
List<int> Indices { get; set; } 
```
Indices of this face forPolygonMesh.Vertices.
```c#
Material Material { get; set; } 
```
Render material for this face.
