# ScenePortal

## ```c#
Derives from SceneObject
```

## Summary

Renders a view within aSandbox.SceneWorldonto a texture on a model.
The model requires a material with $MonitorTexture dynamic expression on one of its textures, usually "Color", to function properly.
## Constructors

```c#
ScenePortal( SceneWorld world, Model model, Transform transform, bool useHDRBuffer = false, int rtSize = 512) 
```
Initializes a new scene portal.
## Properties

```c#
float Aspect { get; set; } 
```
Aspect ratio for the render.
```c#
Color ClearColor { set; } 
```
Color to clear theScenePortal.ColorTargetto before each render.
```c#
Texture ColorTarget { get; } 
```
Render target containing the color information.
```c#
Texture DepthTarget { get; } 
```
Render target containing the depth buffer information.
```c#
float FieldOfView { get; set; } 
```
The horizontal field of view of the Camera in degrees.
```c#
bool IsValid { get; } 
```
ImplementsIValid.IsValidWhether this object is valid or not.
```c#
bool RenderShadows { get; set; } 
```
Whether to render shadows in the scene or not.
```c#
RenderAttributes SceneAttributes { get; init; } 
```
No Summary
```c#
Vector3 ViewPosition { get; set; } 
```
The position of the scene's camera.
```c#
Rotation ViewRotation { get; set; } 
```
The rotation of the scene's camera.
```c#
float ZFar { get; set; } 
```
The camera's zFar distance. This is the furthest distance this camera will be able to render.
This value totally depends on the game you're making. Shorter the better, sensible ranges would be
between about 1000 and 30000, but if you want it to be further out you can balance that out by making
znear larger.
```c#
float ZNear { get; set; } 
```
The camera's zNear distance. This is the closest distance this camera will be able to render.
A good value for this is about 5. Below 5 and particularly below 1 you're going to start to see
a lot of artifacts like z-fighting.
## Methods

```c#
void SetClipPlane( Plane clipPlane) 
```
Sets a render clipping plane.
## Inheriting Types

