# SceneLayerType

## Derives from Enum

## Summary

Depth prepass to reduce overdraw
## Fields

```c#
static SceneLayerType DepthPrepass = 7
```
Depth prepass to reduce overdraw
```c#
static SceneLayerType EffectsOpaque = 6
```
Opaque effects on the 1/4 texture
```c#
static SceneLayerType EffectsTranslucent = 5
```
Translucent effects on the 1/4 texture
```c#
static SceneLayerType Opaque = 8
```
No Summary
```c#
static SceneLayerType Shadow = 4
```
Rendering dynamic shadows
```c#
static SceneLayerType Translucent = 1
```
Translucent pass. We're rendering translucent objects in depth sorted order, from back to front.
```c#
static SceneLayerType Unknown = 0
```
No Summary
## Referencing Members

```c#
static SceneLayerType = Graphics.LayerType { get; } 
```
