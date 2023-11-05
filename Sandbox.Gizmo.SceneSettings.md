# SceneSettings

## 
```c#
Derives from object
```

## Summary

Camera field of view
## Constructors

```c#
SceneSettings( ) 
```
No Summary
## Properties

```c#
float CameraFieldOfView { get; set; } 
```
Camera field of view
```c#
float CameraMovementSmoothing { get; set; } 
```
Should we smooth the movement of the camera. This is the smooth time, in seconds. No smoothing
feels pretty jarring, but a bit feels nice. Once you get over half a second it makes everything feel
slow and horrible.
```c#
bool CameraOrthographic { get; set; } 
```
Is the camera orthographic or perspective
```c#
float CameraSpeed { get; set; } 
```
How fast should the camera move
```c#
float CameraZFar { get; set; } 
```
The furthest thing to render
```c#
float CameraZNear { get; set; } 
```
The closest thing to render
```c#
string EditMode { get; set; } 
```
How do we want to edit this? Usually something like "position", "rotation", "scale" etc
```c#
float GimzoScale { get; set; } 
```
How big to show the gizmos
```c#
bool GlobalSpace { get; set; } 
```
Editing in local space
```c#
string ViewMode { get; set; } 
```
What is the current view mode? 3d, 2d, ui?
