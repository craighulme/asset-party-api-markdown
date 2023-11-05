# ModelBuilder

## ```c#
Derives from object
```

## Summary

Provides ability to generateSandbox.Models at runtime.
A static instance of this class is available atModel.Builder
## Constructors

```c#
ModelBuilder( ) 
```
No Summary
## Methods

```c#
void AddBone( Bone bone) 
```
Add a bone to the skeleton via aModelBuilder.Bonestruct.
```c#
ModelBuilder AddBone( string name, Vector3 position, Rotation rotation, string parentName = null) 
```
Add a bone to the skeleton.
```c#
void AddBones( Bone[] bones) 
```
Add multiple bones to the skeleton.
```c#
ModelBuilder AddCollisionBox( Vector3 extents, Vector3? center = null, Rotation? rotation = null) 
```
Add box collision shape.
```c#
ModelBuilder AddCollisionCapsule( Vector3 center0, Vector3 center1, float radius) 
```
Add capsule collision shape.
```c#
ModelBuilder AddCollisionHull( Vector3[] vertices, Vector3? center = null, Rotation? rotation = null) 
```
Add a CONVEX hull collision shape.
```c#
ModelBuilder AddCollisionMesh( Vector3[] vertices, int[] indices) 
```
Add a CONCAVE mesh collision shape. (This shape can NOT be physically simulated)
```c#
ModelBuilder AddCollisionSphere( float radius, Vector3 center = null) 
```
Add sphere collision shape.
```c#
ModelBuilder AddMesh( Mesh mesh) 
```
Add a mesh.
```c#
ModelBuilder AddMesh( Mesh mesh, int lod) 
```
Add a mesh to a Level of Detail (LOD) group.
```c#
ModelBuilder AddMeshes( Mesh[] meshes) 
```
Add a bunch of meshes.
```c#
ModelBuilder AddMeshes( Mesh[] meshes, int lod) 
```
Add a bunch of meshes to a Level of Detail (LOD) group.
```c#
Model Create( ) 
```
Finish creation of the model.
```c#
ModelBuilder WithLodDistance( float distance) 
```
LOD switch distance increment for each Level of Detail (LOD) level. (Default is 50)
```c#
ModelBuilder WithMass( float mass) 
```
Total mass of the physics body (Default is 1000)
```c#
ModelBuilder WithSurface( string name) 
```
Surface property to use for collision
## Nested Types

