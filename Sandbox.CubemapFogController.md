# CubemapFogController

## ```c#
Derives from object
```

## Summary

Is this cubemap fog active?
## Constructors

```c#
CubemapFogController( ) 
```
No Summary
## Properties

```c#
bool Enabled { get; set; } 
```
Is this cubemap fog active?
```c#
float EndDistance { get; set; } 
```
The distance from the player at which the fog will be at full strength.
```c#
float FalloffExponent { get; set; } 
```
Exponent for distance falloff. For example, 2.0 is proportional to square of distance.
```c#
float HeightExponent { get; set; } 
```
Exponent for height falloff. For example, 2.0 is proportional to square of distance.
```c#
float HeightStart { get; set; } 
```
The absolute height in the map at which the height fog will start to fade in.
```c#
float HeightWidth { get; set; } 
```
The distance between the start of the height fog and where it is fully opaque. Setting this to 0 will disable height based blending.
```c#
float LodBias { get; set; } 
```
Adjust how quickly the cubemap blurs out at closer distances. A value of 0.0 always uses the lowest resolution MIP over the entire range, while a value of 1.0 uses the highest.
```c#
float StartDistance { get; set; } 
```
The distance from the player at which the fog will start to fade in.
```c#
Texture Texture { get; set; } 
```
Cubemap texture to use for the fog.
```c#
Transform Transform { get; set; } 
```
Location of the fog.
