# Plane

## Derives from ValueType
Implements IEquatable< Plane>

## Summary

Represents a plane.
## Constructors

```c#
Plane( Vector3 normal, double dist) 
```
No Summary
```c#
Plane( Vector3 origin, Vector3 normal) 
```
No Summary
```c#
Plane( Vector3 origin, Vector3 posA, Vector3 posB) 
```
Creates a new plane from 3 given positions.
## Fields

```c#
float Distance
```
Distance of the plane from world origin in the direction given byPlane.Normal.
```c#
Vector3 Normal
```
The direction of the plane.
## Properties

```c#
Vector3 Origin { get; } 
```
Origin position of the plane, basically a vectorPlane.Distanceaway from world origin in the direction given byPlane.Normal.
## Methods

```c#
static Vector3? GetIntersection( Plane vp1, Plane vp2, Plane vp3) 
```
Gets the intersecting point of the three planes if it exists.
If the planes don't all intersect will return null.
```c#
float GetDistance( Vector3 point) 
```
Returns the distance from this plane to given point.
```c#
bool IsInFront( Vector3 point) 
```
Returns true if given point is on the side of the plane where its normal is pointing.
```c#
bool IsInFront( BBox box, bool partially = false) 
```
Returns true if given bounding box is on the side of the plane where its normal is pointing.
```c#
Vector3 SnapToPlane( Vector3 point) 
```
Returns closest point on the plane to given point.
```c#
Vector3? Trace( Ray ray, bool twosided = false, double maxDistance = 1.7976931348623157E+308) 
```
Trace a Ray against this plane
```c#
bool TryTrace( Ray ray, out Vector3 hitPoint, bool twosided = false, double maxDistance = 1.7976931348623157E+308) 
```
Trace a Ray against this plane
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( Plane o) 
```
OverridesValueType.Equals
```c#
override int GetHashCode( ) 
```
OverridesValueType.GetHashCode
## Operators

```c#
bool ==( Plane left, Plane right) 
```
No Summary
```c#
bool !=( Plane left, Plane right) 
```
No Summary
## Referencing Members

```c#
Plane = Frustum.BottomPlane
```
```c#
Plane = SceneObject.ClipPlane { get; set; } 
```
```c#
Plane = Frustum.FarPlane
```
```c#
Plane = Frustum.LeftPlane
```
```c#
Plane = Frustum.NearPlane
```
```c#
Matrix = PlanarReflection.ReflectMatrix( Matrix, Plane ) 
```
```c#
Plane = Frustum.RightPlane
```
```c#
void ScenePortal.SetClipPlane( Plane ) 
```
```c#
Plane = Frustum.TopPlane
```
