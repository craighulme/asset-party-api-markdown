# Sphere

## Derives from ValueType

## Summary

Represents a sphere.
## Constructors

```c#
Sphere( Vector3 center, float radius) 
```
No Summary
## Properties

```c#
static Sphere Unit { get; } 
```
A sphere centered at the origin, with radius 1.
```c#
Vector3 Center { get; set; } 
```
Center of the sphere.
```c#
float Radius { get; set; } 
```
Radius of the sphere.
## Methods

```c#
bool Trace( Ray ray, double maxDistance = 1.7976931348623157E+308) 
```
No Summary
```c#
bool Trace( Ray ray, float maxDistance, out float distance) 
```
Performs an intersection test between this sphere and given ray.
```c#
override string ToString( ) 
```
OverridesValueType.ToString
## Referencing Members

```c#
void GizmoHitbox.Sphere( Sphere ) 
```
```c#
Sphere = SpherePart.Sphere { get; init; } 
```
```c#
void DebugOverlay.Sphere( Sphere, Color, float ) 
```
