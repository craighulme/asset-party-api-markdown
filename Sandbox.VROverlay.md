# VROverlay

## 
```c#
Implements IDisposable
```

## Summary

VR overlays draw over the top of the 3D scene, they will not be affected by lighting,
post processing effects or anything else in the world.This makes them ideal for HUDs or menus, or anything else that should be local to the
HMD or tracked devices.If you need something in the world, consider using WorldPanel
andUI.WorldInputinstead.
## Constructors

```c#
VROverlay( ) 
```
No Summary
## Properties

```c#
Color Color { get; set; } 
```
Sets the color tint of the overlay quad. Use 0.0 to 1.0 per channel.
Sets the alpha of the overlay quad. Use 1.0 for 100 percent opacity to 0.0 for 0 percent opacity.
```c#
float Curvature { get; set; } 
```
Use to draw overlay as a curved surface. Curvature is a percentage from (0..1] where 1 is a fully closed cylinder.
For a specific radius, curvature can be computed as: overlay.width / (2 PI r).
```c#
Vector2 MouseScale { get; set; } 
```
No Summary
```c#
uint SortOrder { set; } 
```
No Summary
```c#
Texture Texture { get; set; } 
```
Texture that is rendered on the overlay quad.Sandbox.TextureBuilder
```c#
Transform Transform { get; set; } 
```
Sets the transform to absolute tracking origin
```c#
bool Visible { get; set; } 
```
Shows or hides the VR overlay.
```c#
float Width { get; set; } 
```
The width of the overlay quad.
By default overlays are rendered on a quad that is 1 meter across.
## Methods

```c#
virtual void Dispose( ) 
```
ImplementsIDisposable.Dispose
```c#
protected virtual void Dispose( bool disposing) 
```
No Summary
```c#
void SetHudTransform( Transform tx) 
```
No Summary
```c#
void SetTransformAbsolute( Transform transform) 
```
Sets the transform to absolute tracking origin
```c#
void SetTransformRelative( VROverlay relativeOverlay, Transform transform) 
```
Sets the transform to relative to the transform of the specified overlay. This overlays visibility will also track the parents visibility.
```c#
void SetTransformRelative( VRTrackedDevice relativeTrackedDevice, Transform transform) 
```
No Summary
## Inheriting Types

