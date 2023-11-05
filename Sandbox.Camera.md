# Camera

## ```c#
Derives from object
```

## Summary

Global accessor for the current game's camera
## Properties

```c#
static SceneCamera Current { get; } 
```
The camera that is current being rendered - else null
```c#
static float FieldOfView { get; set; } 
```
The current camera's horizontal field of view in degrees. If current is null, falls back to main camera.
```c#
static IEntity FirstPersonViewer { get; set; } 
```
The current camera's first person viewer. If set then the entity that is viewing
will be invisible, and entities marked as viewmodels will be visible.
```c#
static SceneCamera Main { get; } 
```
The current game's camera, which is used to render the main view
```c#
static Vector3 Position { get; set; } 
```
The current camera's position. If current is null, falls back to main camera.
```c#
static Rotation Rotation { get; set; } 
```
The current camera's rotation. If current is null, falls back to main camera.
```c#
static Vector2 Size { get; } 
```
The current camera's size (in pixels)
```c#
static float ZFar { get; set; } 
```
The current camera's far plane. If current is null, falls back to main camera.
```c#
static float ZNear { get; set; } 
```
The current camera's far plane. If current is null, falls back to main camera.
