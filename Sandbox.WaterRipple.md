# WaterRipple

## 
```c#
Derives from SceneCustomObject
```

## Summary

How far is the simulation radius of the splash from camera view
## Constructors

```c#
WaterRipple( SceneWorld world, Water parent) 
```
No Summary
## Fields

```c#
RippleCascade Cascade
```
No Summary
```c#
float Radius
```
How far is the simulation radius of the splash from camera view
```c#
RippleConstants SplashConstants
```
No Summary
## Methods

```c#
void AddRipple( Vector2 position, Vector2 velocity, float force, float radius = 2) 
```
No Summary
```c#
void OnRender( ) 
```
Renders the splash texture on the compute shader on the GPU
```c#
void Update( ) 
```
Updates per frame data for the splash to render on the GPU next
```c#
override void RenderSceneObject( ) 
```
OverridesSceneCustomObject.RenderSceneObjectCalled when this scene object needs to be rendered.
InvokesSceneCustomObject.RenderOverrideby default. See theSandbox.Graphicslibrary for a starting point.
## Nested Types

