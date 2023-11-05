# MapMesh

## ```c#
Derives from MapNode
```

## Summary

MapMesh is the Hammer map node which represents editable mesh geometry in a Hammer map.
This is the map node that is created when using the hammer geometry editing tools.
## Constructors

```c#
MapMesh( MapDocument mapDocument = null) 
```
No Summary
## Methods

```c#
void ConstructFromPolygons( PolygonMesh polygonMesh) 
```
Constructs the mesh from the givenMapDoc.PolygonMeshbuilder.
```c#
IEnumerable<Asset> GetFaceMaterialAssets( ) 
```
Get all material assets used on this mesh
```c#
void SetMaterial( Material material) 
```
Assigns the specified material to the entire mesh
## Inheriting Types

