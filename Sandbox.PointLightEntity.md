# PointLightEntity

## 
```c#
Derives from ModelEntity
```

## Summary

An omni-directional light entity.
## Constructors

```c#
PointLightEntity( ) 
```
No Summary
## Properties

```c#
float Brightness { get; set; } 
```
Brightness of this light.
```c#
float BrightnessMultiplier { get; set; } 
```
Brightness multiplier.
```c#
Color Color { get; set; } 
```
Color of this light.
```c#
bool DynamicShadows { get; set; } 
```
Enable or disable dynamic shadow casting.
```c#
bool Enabled { get; set; } 
```
Whether this light is enabled or not.
```c#
float FadeDistanceMax { get; set; } 
```
Maximum distance at which the light is visible. (0 = don't fade out)
```c#
float FadeDistanceMin { get; set; } 
```
Distance at which the light starts to fade. (less than 0 = use 'Fade Distance Max')
```c#
float Falloff { get; set; } 
```
Angular falloff exponent. Does not work with light cookies. Does not work with dynamic lighting.
```c#
bool Flicker { get; set; } 
```
Flicker the light 8 times a second.
```c#
float FogStrength { get; set; } 
```
Overrides how much the light affects the fog. (if enabled)
```c#
float LightSize { get; set; } 
```
No Summary
```c#
float LinearAttenuation { get; set; } 
```
No Summary
```c#
float QuadraticAttenuation { get; set; } 
```
No Summary
```c#
float Range { get; set; } 
```
Distance range for light. 0=infinite
```c#
float ShadowFadeDistanceMax { get; set; } 
```
Maximum distance at which the shadow is visible. (0 = don't fade out)
```c#
float ShadowFadeDistanceMin { get; set; } 
```
Distance at which the shadow starts to fade. (less than 0 = use 'Shadow End Fade Dist')
```c#
override SceneLight SceneObject { get; } 
```
OverridesModelEntity.SceneObjectTheModelEntity.SceneObjectthat represents this entity.
## Methods

```c#
protected void SetDefaults( ) 
```
No Summary
```c#
void SetLightBrightness( float brightness) 
```
Set the light brightness.
```c#
void SetLightColor( Color color) 
```
Set the color of the light.
```c#
void SetLightEnabled( bool state) 
```
Turn the light on or off via the parameter.
```c#
void Toggle( ) 
```
Toggle the light on or off.
```c#
void TurnOff( ) 
```
Turn the light off.
```c#
void TurnOn( ) 
```
Turn the light on.
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
## Inheriting Types

