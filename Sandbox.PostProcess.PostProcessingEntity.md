# PostProcessingEntity

## 
```c#
Implements IPostProcessEntity
```

## Summary

Applies given post processing effect to all players. Only the last activated entity will have an effect. (works like a stack)
Overridden bypost processing volume.
## Constructors

```c#
PostProcessingEntity( ) 
```
No Summary
## Properties

```c#
virtual bool Enabled { get; set; } 
```
ImplementsIPostProcessEntity.EnabledWhether this entity is enabled.
```c#
virtual bool EnableExposure { get; set; } 
```
ImplementsIPostProcessEntity.EnableExposureUse exposure settings for this entity
```c#
virtual float ExposureCompensation { get; set; } 
```
ImplementsIPostProcessEntity.ExposureCompensationNumber of stops to adjust auto-exposure by
```c#
virtual float ExposureFadeSpeedDown { get; set; } 
```
ImplementsIPostProcessEntity.ExposureFadeSpeedDown
```c#
virtual float ExposureFadeSpeedUp { get; set; } 
```
ImplementsIPostProcessEntity.ExposureFadeSpeedUp
```c#
virtual float FadeTime { get; set; } 
```
ImplementsIPostProcessEntity.FadeTimeTime to fade to these post-processing settings in seconds
```c#
virtual float MaxExposure { get; set; } 
```
ImplementsIPostProcessEntity.MaxExposureMaximum auto exposure scale
```c#
virtual float MinExposure { get; set; } 
```
ImplementsIPostProcessEntity.MinExposureMinimum auto exposure scale
```c#
virtual float PercentBrightPixels { get; set; } 
```
ImplementsIPostProcessEntity.PercentBrightPixelsSet a target for percentage of pixels above a certain brightness. (-1 for default engine behavior)
```c#
virtual float PercentTarget { get; set; } 
```
ImplementsIPostProcessEntity.PercentTargetSet a custom brightness target to go along with 'Target Bright Pixel Percentage'. (-1 for default engine behavior)
```c#
virtual string PostProcessingFile { get; set; } 
```
ImplementsIPostProcessEntity.PostProcessingFileThe post process resource file to use
```c#
virtual float TonemapMinAvgLum { get; set; } 
```
ImplementsIPostProcessEntity.TonemapMinAvgLum
## Methods

```c#
void Disable( ) 
```
Disable this post processing effect.
```c#
void Enable( ) 
```
Enable this post processing effect.
```c#
protected void TurnOffEffect( ) 
```
No Summary
```c#
protected void TurnOffEffect( To toTarget) 
```
No Summary
```c#
protected void TurnOnEffect( ) 
```
No Summary
```c#
protected void TurnOnEffect( To toTarget) 
```
No Summary
```c#
override void ClientSpawn( ) 
```
OverridesEntity.ClientSpawnCalled when the entity spawns on client.
```c#
protected override void OnDestroy( ) 
```
OverridesEntity.OnDestroyCalled when the entity was destroyed. This is not the same as the class destructor.
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
## Inheriting Types

