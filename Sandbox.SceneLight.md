# SceneLight

## ```c#
Derives from SceneObject
```

## Summary

Generic point light scene object for use with aSandbox.SceneWorld.
## Constructors

```c#
SceneLight( SceneWorld sceneWorld, Vector3 position, float radius, Color color) 
```
No Summary
```c#
SceneLight( SceneWorld sceneWorld) 
```
No Summary
## Properties

```c#
float ConstantAttenuation { get; set; } 
```
The light attenuation constant term
```c#
FogLightingMode FogLighting { get; set; } 
```
No Summary
```c#
Color LightColor { get; set; } 
```
Color and brightness of the light
```c#
Texture LightCookie { get; set; } 
```
Access the LightCookie - which is a texture that gets drawn over the light
```c#
float LinearAttenuation { get; set; } 
```
The light attenuation linear term
```c#
float QuadraticAttenuation { get; set; } 
```
The light attenuation quadratic term
```c#
float Radius { get; set; } 
```
Radius of the light in units
```c#
bool ShadowsEnabled { get; set; } 
```
Enable or disable shadow rendering
```c#
int ShadowTextureResolution { get; set; } 
```
Get or set the resolution of the shadow map. If this is zero the engine will decide what it should use.
## Nested Types

## Inheriting Types

