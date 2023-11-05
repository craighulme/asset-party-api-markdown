# Frustum

## 
```c#
Implements IEquatable<Frustum>
```

## Summary

Represents afrustum.
## Fields

```c#
Plane BottomPlane
```
Bottom plane of the frustum, pointing inwards.
```c#
Plane FarPlane
```
Far plane of the frustum, pointing inwards.
```c#
Plane LeftPlane
```
Left plane of the frustum, pointing inwards.
```c#
Plane NearPlane
```
Near plane of the frustum, pointing inwards.
```c#
Plane RightPlane
```
Right plane of the frustum, pointing inwards.
```c#
Plane TopPlane
```
Top plane of the frustum, pointing inwards.
## Methods

```c#
BBox GetBBox( ) 
```
Returns the AABB of this frustum.
```c#
Vector3? GetCorner( int i) 
```
Returns the corner point of one of the 8 corners.
This may return null if i is > 7 or the frustum is invalid.
```c#
bool IsInside( Vector3 point) 
```
Returns whether the given point is inside this frustum.
```c#
bool IsInside( BBox box, bool partially = false) 
```
Returns whether given AABB is inside this frustum.
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( Frustum o) 
```
OverridesValueType.Equals
```c#
override int GetHashCode( ) 
```
OverridesValueType.GetHashCode
## Operators

```c#
bool ==( Frustum left, Frustum right) 
```
No Summary
```c#
bool !=( Frustum left, Frustum right) 
```
No Summary
