# ScenePanelObject

## Derives from SceneCustomObject

## Summary

Renders a panel in a scene world. You are probably looking forWorldPanel.
## Constructors

```c#
ScenePanelObject( SceneWorld world, RootPanel Panel) 
```
No Summary
## Fields

```c#
static float ScreenToWorldScale = 0.05
```
Global scale for panel rendering within a scene world.
## Properties

```c#
RootPanel Panel { get; } 
```
The panel that will be rendered.
## Methods

```c#
override void RenderSceneObject( ) 
```
OverridesSceneCustomObject.RenderSceneObjectCalled when this scene object needs to be rendered.
InvokesSceneCustomObject.RenderOverrideby default. See theSandbox.Graphicslibrary for a starting point.
