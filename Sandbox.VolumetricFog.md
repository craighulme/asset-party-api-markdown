# VolumetricFog

## 
```c#
Derives from object
```

## Summary

Level of anisotropy.
## Properties

```c#
float Anisotropy { get; set; } 
```
Level of anisotropy.
```c#
Texture BakedIndirectTexture { get; set; } 
```
Provides indirect lighting from a baked volume texture.
This gets compiled with your map and is provided by an env_volumetric_controller.
```c#
bool ContinuousMode { get; set; } 
```
Indicates if the fog system operates in continuous mode.
This means the clipmaps update every frame.
```c#
float DrawDistance { get; set; } 
```
Draw distance.
```c#
bool Enabled { get; set; } 
```
Indicates whether the fog system is enabled.
```c#
float FadeInEnd { get; set; } 
```
End distance where fading concludes.
```c#
float FadeInStart { get; set; } 
```
Start distance where fading begins.
```c#
float IndirectStrength { get; set; } 
```
Strength of indirect illumination.
```c#
float Scattering { get; set; } 
```
Scattering value.
