# Ray

## ```c#
Implements IEquatable<Ray>
```

## Summary

A struct describing an origin and direction
## Constructors

```c#
Ray( Vector3 origin, Vector3 direction) 
```
No Summary
## Properties

```c#
Vector3 Forward { get; set; } 
```
Direction of the ray.
```c#
Vector3 Position { get; set; } 
```
Origin of the ray.
## Methods

```c#
static Ray Read( BinaryReader reader) 
```
Read aRayfrom given binary reader.
```c#
Vector3 Project( float distance) 
```
Returns a point on the ray at given distance.
```c#
Ray ToLocal( in Transform tx) 
```
Convert a ray to be local to this transform
```c#
Ray ToWorld( in Transform tx) 
```
Convert a ray from being local to this transform
```c#
void Write( BinaryWriter writer) 
```
Write this ray to a System.IO.BinaryWriter.
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( Ray o) 
```
OverridesValueType.Equals
```c#
override int GetHashCode( ) 
```
OverridesValueType.GetHashCode
## Operators

```c#
bool ==( Ray left, Ray right) 
```
No Summary
```c#
bool !=( Ray left, Ray right) 
```
No Summary
## Referencing Members

```c#
static void SandboxBaseExtensions.AddQuad( VertexBuffer, Ray, Vector3, Vector3 ) 
```
```c#
abstract Ray = IEntity.AimRay { get; } 
```
```c#
virtual Ray = Entity.AimRay { get; } 
```
```c#
override Ray = Player.AimRay { get; } 
```
```c#
static Ray = Gizmo.CurrentRay { get; } 
```
```c#
Ray = Inputs.CursorRay { get; set; } 
```
```c#
Ray = NativeRenderingWidget.CursorRay { get; } 
```
```c#
static Ray = Screen.GetOrthoRay( Vector2 ) 
```
```c#
static Vector3? = Gizmo.GetPositionOnPlane( Vector3, Vector3, Ray ) 
```
```c#
Ray = SceneCamera.GetRay( Vector3 ) 
```
```c#
Ray = SceneCamera.GetRay( Vector3, Vector3 ) 
```
```c#
Ray = NativeRenderingWidget.GetRay( Vector2 ) 
```
```c#
virtual bool = BaseGameManager.OnDragDropped( string, Ray, string ) 
```
```c#
static Ray = Gizmo.PressRay { get; } 
```
```c#
static Ray = Gizmo.PreviousRay { get; } 
```
```c#
Ray = WorldInput.Ray { get; set; } 
```
```c#
virtual bool = Panel.RayToLocalPosition( Ray, out Vector2, out float ) 
```
```c#
override bool = WorldPanel.RayToLocalPosition( Ray, out Vector2, out float ) 
```
```c#
static Ray = SandboxSystemExtensions.ReadRay( BinaryReader ) 
```
```c#
bool = BBox.Trace( Ray, float, out float ) 
```
```c#
Vector3? = Plane.Trace( Ray, bool, double ) 
```
```c#
bool = Sphere.Trace( Ray, double ) 
```
```c#
bool = Sphere.Trace( Ray, float, out float ) 
```
```c#
bool = Plane.TryTrace( Ray, out Vector3, bool, double ) 
```
```c#
static void SandboxSystemExtensions.Write( BinaryWriter, Ray ) 
```
