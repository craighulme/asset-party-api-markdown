# SceneFogVolume

## Derives from object
Implements IValid

## Summary

Represents a volume of fog in a scene, contributing to volumetric fog effects set onSceneCamera.VolumetricFog.
## Constructors

```c#
SceneFogVolume( SceneWorld world, Transform transform, BBox boundingBox, float fogStrength = 1, float falloffExponent = 1) 
```
No Summary
## Properties

```c#
virtual bool IsValid { get; } 
```
ImplementsIValid.IsValidWhether this object is valid or not.
```c#
BBox BoundingBox { get; set; } 
```
Defines the spatial boundaries of the fog volume.
```c#
float FalloffExponent { get; set; } 
```
Controls how quickly the fog fades at the edges of the volume. Higher values give sharper transitions.
```c#
float FogStrength { get; set; } 
```
The intensity of the fog. Higher values indicate denser fog.
```c#
Transform Transform { get; set; } 
```
The position and rotation of the fog volume in the scene.
## Methods

```c#
void Delete( ) 
```
Delete this fog volume. You shouldn't access it anymore.
