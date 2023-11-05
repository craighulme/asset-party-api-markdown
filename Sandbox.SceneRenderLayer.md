# SceneRenderLayer

## Derives from Enum

## Summary

SceneObjects can be rendered on layers other than the main game layer.
This is useful if, for example, you want to render on top of everything without
applying post processing.
## Fields

```c#
static SceneRenderLayer Default = 0
```
Draw wherever makes sense based on the flags, default behaviour
```c#
static SceneRenderLayer OverlayWithDepth = 20
```
Overlay - after post processing - but still with the scene's depth
```c#
static SceneRenderLayer OverlayWithoutDepth = 30
```
Overlay - after post processing - without depth (draw over)
```c#
static SceneRenderLayer ViewModel = 10
```
Layer drawn on top of everything else - with altered depth
## Referencing Members

```c#
SceneRenderLayer = SceneObject.RenderLayer { get; set; } 
```
