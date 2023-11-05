# SceneSunLight

## Derives from SceneLight

## Summary

A directional scene light that is used to mimic sun light in aSandbox.SceneWorld. Direction is controlled by this objects'Rotation.
## Constructors

```c#
SceneSunLight( SceneWorld sceneWorld, Rotation rotation, Color color) 
```
No Summary
## Properties

```c#
int ShadowCascadeCount { get; set; } 
```
Control number of shadow cascades
```c#
Color SkyColor { get; set; } 
```
No Summary
## Methods

```c#
void SetShadowCascadeDistance( int cascade_index, float distance) 
```
Set the max distance of the shadow cascade
```c#
void SetShadowCascadeResolution( int cascade_index, int resolution) 
```
Set the resolution of the shadow cascade. Defaults start at 2048
