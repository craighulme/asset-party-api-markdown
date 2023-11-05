# GradientFogEntity

## 
```c#
Derives from ModelEntity
```

## Summary

Specifies fog based on a color gradient
## Constructors

```c#
GradientFogEntity( ) 
```
No Summary
## Properties

```c#
Color FogColor { get; set; } 
```
Set the gradient fog color.
```c#
float FogDistanceFalloffExponent { get; set; } 
```
Exponent for distance falloff.
```c#
bool FogEnabled { get; set; } 
```
Whether the fog is enabled or not.
```c#
float FogEndDistance { get; set; } 
```
Fog end distance.
```c#
float FogEndHeight { get; set; } 
```
Fog end height.
```c#
float FogFadeTime { get; set; } 
```
How much time it takes to fade in new values.
```c#
float FogMaximumOpacity { get; set; } 
```
Set the maximum opacity at the base of the gradient fog.
```c#
float FogStartDistance { get; set; } 
```
For start distance.
```c#
float FogStartHeight { get; set; } 
```
Fog start height.
```c#
float FogStrength { get; set; } 
```
Fog strength.
```c#
float FogVerticalFalloffExponent { get; set; } 
```
"Exponent for vertical falloff."
## Methods

```c#
void SetFogColor( Color fogColor) 
```
Set Fog Color
```c#
void SetFogEndDistance( float fogDistance) 
```
Set Fog End Distance
```c#
void SetFogEndHeight( float height) 
```
Set Fog End Height
```c#
void SetFogFalloffExponent( float exponent) 
```
Set Fog Falloff Exponent
```c#
void SetFogMaxOpacity( float maxOpacity) 
```
Set Fog Max Opacity
```c#
void SetFogStartDistance( float fogDistance) 
```
Set Fog Start Distance
```c#
void SetFogStartHeight( float height) 
```
Set Fog Start Height
```c#
void SetFogStrength( float strength) 
```
Set Fog Strength
```c#
void SetFogVerticalExponent( float exponent) 
```
Set Fog Vertical Exponent
```c#
void UpdateFogState( bool isForceSet = false) 
```
Update fog values on client.
```c#
void UpdateFogState( To toTarget, bool isForceSet = false) 
```
Update fog values on client.
```c#
override void ClientSpawn( ) 
```
OverridesEntity.ClientSpawnCalled when the entity spawns on client.
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
