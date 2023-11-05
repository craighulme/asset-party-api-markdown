# IPostProcessEntity

## Is interface
Inherits IValid

## Summary

Set every frame with the most relevant entity to swap to
## Fields

```c#
static IPostProcessEntity _active
```
Set every frame with the most relevant entity to swap to
## Properties

```c#
abstract bool Enabled { get; } 
```
No Summary
```c#
abstract bool EnableExposure { get; } 
```
Use exposure settings for this entity
```c#
abstract float ExposureCompensation { get; } 
```
Number of stops to adjust auto-exposure by
```c#
abstract float ExposureFadeSpeedDown { get; } 
```
No Summary
```c#
abstract float ExposureFadeSpeedUp { get; } 
```
No Summary
```c#
abstract float FadeTime { get; } 
```
Time to fade to these post-processing settings in seconds
```c#
abstract float MaxExposure { get; } 
```
Maximum auto exposure scale
```c#
abstract float MinExposure { get; } 
```
Minimum auto exposure scale
```c#
abstract float PercentBrightPixels { get; } 
```
Set a target for percentage of pixels above a certain brightness. (-1 for default engine behavior)
```c#
abstract float PercentTarget { get; } 
```
Set a custom brightness target to go along with 'Target Bright Pixel Percentage'. (-1 for default engine behavior)
```c#
abstract string PostProcessingFile { get; } 
```
The post process resource file to use
```c#
abstract float TonemapMinAvgLum { get; } 
```
No Summary
## Methods

```c#
static void Add( IPostProcessEntity effect) 
```
No Summary
```c#
static void Remove( IPostProcessEntity effect) 
```
No Summary
