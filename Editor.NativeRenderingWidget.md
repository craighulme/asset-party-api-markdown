# NativeRenderingWidget

## ```c#
Derives from Frame
```

## Summary

Sets up the widget to render
## Constructors

```c#
NativeRenderingWidget( Widget parent = null) 
```
No Summary
## Properties

```c#
SceneCamera Camera { get; set; } 
```
The camera to render from
```c#
Ray CursorRay { get; } 
```
Return a ray for the current cursor position
```c#
bool RenderEveryFrame { get; set; } 
```
If true we'll attempt to render Camera every frame
## Methods

```c#
virtual void PostFrame( ) 
```
No Summary
```c#
virtual void PreFrame( ) 
```
No Summary
```c#
Ray GetRay( Vector2 localPosition) 
```
Given a local widget position, return a Ray
```c#
void RenderScene( ) 
```
No Summary
## Inheriting Types

