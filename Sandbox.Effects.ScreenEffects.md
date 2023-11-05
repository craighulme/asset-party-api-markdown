# ScreenEffects

## 
```c#
Derives from RenderHook
```

## Summary

Draws the highlight outline effect. You may know this effect from
such games as Garry's Mod.
## Constructors

```c#
ScreenEffects( ) 
```
No Summary
## Properties

```c#
float Brightness { get; set; } 
```
How Bright. Default 1.
```c#
ChromaticAberrationSettings ChromaticAberration { get; } 
```
Chromatic Aberration settings.
```c#
float Contrast { get; set; } 
```
How contrasty
```c#
FilmGrainSettings FilmGrain { get; } 
```
Film grain settings.
```c#
float HueRotate { get; set; } 
```
How much to rotate the hue by, this is a value from 0->360.
The default value for this is 0.0f which means no change
```c#
MotionBlurSettings MotionBlur { get; } 
```
Motion Blur settings.
```c#
float Pixelation { get; set; } 
```
0 for non pixelated, 1 for one big pixel
```c#
float Saturation { get; set; } 
```
How saturated our view should be. A value of
0 is a grayscale result whereas 1 is no change. Any
value greater than 1 will lead to an over-saturated or
"deepfried" look
```c#
float Sharpen { get; set; } 
```
Sharpen the screen
```c#
VignetteSettings Vignette { get; } 
```
Vignette settings.
## Methods

```c#
void RenderEffect( SceneCamera target) 
```
Render the effect onto given scene camera.
```c#
override void OnStage( SceneCamera target, Stage renderStage) 
```
OverridesRenderHook.OnStageCalled while rendering the scene. Check renderStage to find out where.
## Nested Types

