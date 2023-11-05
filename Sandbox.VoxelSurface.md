# VoxelSurface

## ```c#
Derives from ModelEntity
```

## Summary

A procedurally breakable voxel surface.
## Constructors

```c#
VoxelSurface( ) 
```
No Summary
## Properties

```c#
Vector3 FaceAxisForward { get; set; } 
```
No Summary
```c#
Vector3 FaceAxisRight { get; set; } 
```
No Summary
```c#
Vector4 FaceAxisU { get; set; } 
```
No Summary
```c#
Vector4 FaceAxisV { get; set; } 
```
No Summary
```c#
Vector3 FaceCenter { get; set; } 
```
No Summary
```c#
Vector2 FaceTexScale { get; set; } 
```
No Summary
```c#
Vector2 FaceTexSize { get; set; } 
```
No Summary
```c#
string FaceVertices { get; set; } 
```
No Summary
```c#
int Height { get; } 
```
How many voxels on the height (Limited to 64)
```c#
bool IsFrozen { get; } 
```
Is the panel frozen
```c#
string Material { get; set; } 
```
Material to use for the surface
```c#
int NumChunks { get; } 
```
No Summary
```c#
Vector2 Size { get; } 
```
No Summary
```c#
float Thickness { get; } 
```
How thick is the surface (Limited to 64)
```c#
int Width { get; } 
```
How many voxels on the width (Limited to 64)
## Methods

```c#
static void ResetGlassCommand( ) 
```
No Summary
```c#
VoxelChunk CreateNewChunk( ) 
```
No Summary
```c#
void RemoveChunk( VoxelChunk chunk) 
```
No Summary
```c#
void Reset( ) 
```
No Summary
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
