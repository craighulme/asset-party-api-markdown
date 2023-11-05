# DepthOfField

## Derives from RenderHook

## Summary

Draws the highlight outline effect. You may know this effect from
such games as Garry's Mod.
## Constructors

```c#
DepthOfField( ) 
```
No Summary
## Properties

```c#
bool BackBlur { get; set; } 
```
Should we blur what's behind the focal point?
```c#
float BlurSize { get; set; } 
```
How blurry to make stuff that isn't in focus
```c#
float FocalDistance { get; set; } 
```
How far away from the camera to focus
```c#
bool FrontBlur { get; set; } 
```
Should we blur what's ahead the focal point towards us?
## Methods

```c#
void RenderEffect( ) 
```
Render the effect onto given scene camera.
```c#
override void OnStage( SceneCamera target, Stage renderStage) 
```
OverridesRenderHook.OnStageCalled while rendering the scene. Check renderStage to find out where.
