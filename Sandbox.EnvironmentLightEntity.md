# EnvironmentLightEntity

## Derives from Entity

## Summary

An environment light entity. This acts as the sun.
## Constructors

```c#
EnvironmentLightEntity( ) 
```
No Summary
## Properties

```c#
Color AmbientColor { get; set; } 
```
Ambient light color
```c#
float Brightness { get; set; } 
```
Brightness of this light.
```c#
Color Color { get; set; } 
```
Color of this light.
```c#
bool DynamicShadows { get; set; } 
```
Whether this light should cast dynamic shadows.
```c#
bool Enabled { get; set; } 
```
Whether this light is enabled or not.
```c#
float FogStrength { get; set; } 
```
Overrides how much the light affects the fog. (if enabled)
```c#
SceneLight SceneObject { get; } 
```
TheEnvironmentLightEntity.SceneObjectthat represents this entity.
```c#
Color SkyColor { get; set; } 
```
Ambient light color outside of all light probes.
```c#
float SkyIntensity { get; set; } 
```
Ambient light intensity outside of all light probes.
## Methods

```c#
void UseFog( ) 
```
Enable dynamic volumetric fog.
```c#
void UseFogNoShadows( ) 
```
Enable dynamic volumetric fog without shadows.
```c#
void UseNoFog( ) 
```
Disable volumetric fog.
