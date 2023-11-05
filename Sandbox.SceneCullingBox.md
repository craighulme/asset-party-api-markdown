# SceneCullingBox

## ```c#
Implements IValid
```

## Summary

A box which can be used to explicitly control scene visibility.
There are two modes:Cull inside, hide any objects fully inside the box (excluder)Cull outside, hide any objects not intersecting any cull boxes marked cull outside (includer)
## Constructors

```c#
SceneCullingBox( SceneWorld world, Transform transform, Vector3 size, CullMode mode) 
```
Create a scene culling box.
Each scene world can have a list of boxes which can be used to explicitly cull objects inside or outside the boxes.
## Properties

```c#
virtual bool IsValid { get; } 
```
ImplementsIValid.IsValidIs this culling box valid, exists inside a scene world.
```c#
CullMode Mode { get; set; } 
```
Cull mode, either inside or outside
```c#
Vector3 Size { get; set; } 
```
Size of this box, transform scale will scale this size
```c#
Transform Transform { get; set; } 
```
Position and rotation of this box, scale will scale the box size
```c#
SceneWorld World { get; } 
```
The scene world this culling box belongs to.
## Methods

```c#
void Delete( ) 
```
Delete this culling box. You shouldn't access it anymore.
## Nested Types

