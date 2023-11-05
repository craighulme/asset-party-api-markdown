# SpotLightEntity

## Derives from ModelEntity

## Summary

A directional spot light entity.
## Constructors

```c#
SpotLightEntity( ) 
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
float InnerConeAngle { get; set; } 
```
Inner cone angle. No angular falloff within this cone.
```c#
Texture LightCookie { get; set; } 
```
The light cookie texture for this light. A light cookie is like a filter or a mask for the emitted light.
```c#
float LinearAttenuation { get; set; } 
```
No Summary
```c#
float OuterConeAngle { get; set; } 
```
Outer cone angle.
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
