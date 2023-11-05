# TextSceneObject

## 
```c#
Derives from SceneCustomObject
```

## Summary

OverridesSceneCustomObject.RenderSceneObjectCalled when this scene object needs to be rendered.
InvokesSceneCustomObject.RenderOverrideby default. See theSandbox.Graphicslibrary for a starting point.
## Constructors

```c#
TextSceneObject( SceneWorld sceneWorld) 
```
No Summary
## Properties

```c#
string FontName { get; set; } 
```
No Summary
```c#
float FontSize { get; set; } 
```
No Summary
```c#
float FontWeight { get; set; } 
```
No Summary
```c#
string Text { get; set; } 
```
No Summary
```c#
TextFlag TextFlags { get; set; } 
```
No Summary
## Methods

```c#
override void RenderSceneObject( ) 
```
OverridesSceneCustomObject.RenderSceneObjectCalled when this scene object needs to be rendered.
InvokesSceneCustomObject.RenderOverrideby default. See theSandbox.Graphicslibrary for a starting point.
