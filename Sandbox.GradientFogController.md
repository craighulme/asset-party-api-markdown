# GradientFogController

## Derives from ValueType

## Summary

Whether the fog is enabled.
## Properties

```c#
Color Color { get; set; } 
```
No Summary
```c#
float DistanceFalloffExponent { get; set; } 
```
No Summary
```c#
bool Enabled { get; set; } 
```
Whether the fog is enabled.
```c#
float EndDistance { get; set; } 
```
End distance of the fog.
```c#
float EndHeight { get; set; } 
```
No Summary
```c#
float MaximumOpacity { get; set; } 
```
No Summary
```c#
float StartDistance { get; set; } 
```
Start distance of the fog.
```c#
float StartHeight { get; set; } 
```
No Summary
```c#
float VerticalFalloffExponent { get; set; } 
```
No Summary
## Methods

```c#
GradientFogController LerpTo( GradientFogController desired, float delta, bool clamp = true) 
```
No Summary
```c#
void Write( RenderAttributes attr) 
```
No Summary
## Referencing Members

```c#
GradientFogController = SceneWorld.GradientFog
```
