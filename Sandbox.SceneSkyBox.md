# SceneSkyBox

## 
```c#
Derives from SceneObject
```

## Summary

Renders a skybox within aSandbox.SceneWorld.
## Constructors

```c#
SceneSkyBox( SceneWorld world, Material skyMaterial) 
```
No Summary
## Properties

```c#
FogParamInfo FogParams { get; set; } 
```
Controls the skybox specific fog.
```c#
Material SkyMaterial { set; } 
```
The skybox material. Typically it should use the "Sky" shader.
```c#
Color SkyTint { get; set; } 
```
Skybox color tint.
## Methods

```c#
void SetSkyLighting( Vector3 ConstantSkyLight) 
```
No Summary
## Nested Types

