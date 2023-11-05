# Gizmo

## 
```c#
Derives from object
```

## Summary

Holds fully realized controls to manipulate some value
## Properties

```c#
static SceneCamera Camera { get; } 
```
No Summary
```c#
static GizmoControls Control { get; } 
```
Holds fully realized controls to manipulate some value
```c#
static string ControlMode { get; } 
```
No Summary
```c#
static Ray CurrentRay { get; } 
```
No Summary
```c#
static GizmoDraw Draw { get; } 
```
Draw a shape using the gizmo library
```c#
static bool HasClicked { get; } 
```
No Summary
```c#
static bool HasHovered { get; } 
```
No Summary
```c#
static bool HasPressed { get; } 
```
No Summary
```c#
static bool HasSelected { get; } 
```
No Summary
```c#
static GizmoHitbox Hitbox { get; } 
```
Allows creating a gizmo hitbox which will be interactable using the mouse (or vr deck2 super controller)
```c#
static bool IsChildSelected { get; } 
```
No Summary
```c#
static bool IsHovered { get; } 
```
No Summary
```c#
static bool IsPressed { get; } 
```
No Summary
```c#
static bool IsSelected { get; } 
```
No Summary
```c#
static object Object { get; set; } 
```
No Summary
```c#
static string Path { get; set; } 
```
No Summary
```c#
static Ray PressRay { get; } 
```
No Summary
```c#
static Ray PreviousRay { get; } 
```
No Summary
```c#
static SceneSettings Settings { get; } 
```
No Summary
```c#
static Transform Transform { get; set; } 
```
No Summary
```c#
static bool WasClicked { get; } 
```
No Summary
```c#
static SceneWorld World { get; } 
```
No Summary
## Methods

```c#
static void EndInstance( Instance previous) 
```
No Summary
```c#
static Vector3 GetCursorDelta( ) 
```
No Summary
```c#
static Vector3 GetMouseDelta( Vector3 position, Vector3 planeNormal) 
```
Get the mouse delta at this current position
```c#
static float GetMouseDistance( Vector3 position, Vector3 planeNormal) 
```
Get the distance from a point on a plane
```c#
static float GetMouseDistanceDelta( Vector3 position, Vector3 planeNormal) 
```
Get the distance moved from (or towards) a position on a plane
```c#
static Vector3? GetPositionOnPlane( Vector3 position, Vector3 planeNormal, Ray ray) 
```
Get the distance from a point on a plane
```c#
static IDisposable ObjectScope<T,>( T obj, Transform tx) 
```
Create a new scope - any changes to colors and transforms will be stored
and reverted when exiting the scope.
```c#
static IDisposable Scope( string path, Transform tx) 
```
Create a new scope - any changes to colors and transforms will be stored
and reverted when exiting the scope.
```c#
static IDisposable Scope( string path, Vector3 position) 
```
Create a new scope - any changes to colors and transforms will be stored
and reverted when exiting the scope.
```c#
static IDisposable Scope( string path, Vector3 position, Rotation rotation, float scale = 1) 
```
Create a new scope - any changes to colors and transforms will be stored
and reverted when exiting the scope.
```c#
static IDisposable Scope( string path = null) 
```
Create a new scope - any changes to colors and transforms will be stored
and reverted when exiting the scope.
```c#
static void Select( bool allowUnselect = true, bool allowMultiSelect = true) 
```
No Summary
## Nested Types

