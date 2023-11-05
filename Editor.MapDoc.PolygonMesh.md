# PolygonMesh

## 
```c#
Derives from object
```

## Summary

Describes a set of n-gon polygons used to construct a Hammer mesh.
Any overlapping vertices will be merged ifPolygonMesh.MergeVerticies.
## Constructors

```c#
PolygonMesh( ) 
```
No Summary
## Properties

```c#
List<MeshFace> Faces { get; set; } 
```
All faces of this mesh.
```c#
bool MergeVerticies { get; set; } 
```
Whether to merge overlapping vertices.
```c#
float VertexMergeTolerance { get; set; } 
```
Vertex merge tolerance. SeePolygonMesh.MergeVerticies.
```c#
List<MeshVertex> Vertices { get; set; } 
```
All vertices of this mesh.
## Methods

```c#
MeshFace AddFace( int[] indices) 
```
Adds a new face to the end of the Faces list.
```c#
MeshFace AddFace( MeshVertex[] verticies) 
```
Adds a new face to the end of the Faces list and it's vertices to the end of the Vertices list.
```c#
MeshFace AddFace( Vector3[] positions) 
```
Adds a new face to the end of the Faces list and it's vertices to the end of the Vertices list.
```c#
int AddVertex( MeshVertex vertex) 
```
Adds a new vertex to the end of the Vertex list.
```c#
int AddVertex( Vector3 position) 
```
Adds a new vertex to the end of the Vertices list.
