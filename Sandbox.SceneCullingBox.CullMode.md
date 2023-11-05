# CullMode

## ```c#
Derives from Enum
```

## Summary

Cull mode, either inside or outside
## Fields

```c#
static CullMode Inside = 0
```
Hide any objects fully inside the box
```c#
static CullMode Outside = 1
```
Hide any objects not intersecting any boxes
## Referencing Members

```c#
CullMode = SceneCullingBox.Mode { get; set; } 
```
```c#
SceneCullingBox.SceneCullingBox( SceneWorld, Transform, Vector3, CullMode ) 
```
