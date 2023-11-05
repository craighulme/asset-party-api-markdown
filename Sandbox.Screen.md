# Screen

## 
```c#
Derives from object
```

## Summary

Access screen dimension etc.
TODO: We should probably move this to Sandbox.Local.Screen?
## Properties

```c#
static float Aspect { get; } 
```
The aspect ratio of the screen. Equal to Width/Height
```c#
static float Height { get; } 
```
The height of the game screen. Equal to Screen.y
```c#
static Vector2 Size { get; } 
```
The total size of the game screen
```c#
static float Width { get; } 
```
The width of the game screen. Equal to Screen.x
## Methods

```c#
static float CreateVerticalFieldOfView( float fieldOfView) 
```
Converts a vertical field of view to a horizontal field of view based on the screen aspect ratio.
```c#
static float CreateVerticalFieldOfView( float fieldOfView, float aspectRatio) 
```
Converts a vertical field of view to a horizontal field of view based on the given aspect ratio.
```c#
static Vector3 GetDirection( Vector2 pos) 
```
Gives a direction vector based on the position of the point on the screen. The vector represents the direction
from the camera's position you would travel if you could pass through the screen in that direction.
```c#
static Vector3 GetDirection( Vector2 pos, float fov) 
```
Gives a direction vector based on the position of the point on the screen. The vector represents the direction
from the camera's position you would travel if you could pass through the screen in that direction.
```c#
static Vector3 GetDirection( Vector2 pos, float fov, Rotation lookAngle) 
```
Gives a direction vector based on the position of the point on the screen. The vector represents the direction
from the camera's position you would travel if you could pass through the screen in that direction.
```c#
static Vector3 GetDirection( Vector2 pos, float fov, Rotation lookAngle, Vector2 screenSize) 
```
Gives a direction vector based on the position of the point on the screen. The vector represents the direction
from the camera's position you would travel if you could pass through the screen in that direction.
```c#
static Ray GetOrthoRay( Vector2 position) 
```
If current view is orthographic returns a world space ray from the camera's position in the camera's direction.
