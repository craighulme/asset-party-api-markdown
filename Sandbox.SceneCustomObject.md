# SceneCustomObject

## Derives from SceneObject

## Summary

A scene object that allows custom rendering within a scene world.
## Constructors

```c#
SceneCustomObject( SceneWorld sceneWorld) 
```
No Summary
## Fields

```c#
Action<SceneObject> RenderOverride
```
Called by default version ofSceneCustomObject.RenderSceneObject.
## Methods

```c#
virtual void RenderSceneObject( ) 
```
Called when this scene object needs to be rendered.
InvokesSceneCustomObject.RenderOverrideby default. See theSandbox.Graphicslibrary for a starting point.
## Inheriting Types

