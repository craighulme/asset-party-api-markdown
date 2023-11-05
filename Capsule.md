# Capsule

## 
```c#
Implements IEquatable<Capsule>
```

## Summary

A capsule object, defined by 2 points and a radius. A capsule is a cylinder with round ends (inset half spheres on each end).
## Constructors

```c#
Capsule( Vector3 a, Vector3 b, float r) 
```
No Summary
## Fields

```c#
Vector3 CenterA
```
Position of point A.
```c#
Vector3 CenterB
```
Position of point B.
```c#
float Radius
```
Radius of a capsule.
## Methods

```c#
static Capsule FromHeightAndRadius( float height, float radius) 
```
Creates a capsule where Point A is radius units above the ground and Point B is height minus radius units above the ground.
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( Capsule o) 
```
OverridesValueType.Equals
```c#
override int GetHashCode( ) 
```
OverridesValueType.GetHashCode
## Operators

```c#
bool ==( Capsule left, Capsule right) 
```
No Summary
```c#
bool !=( Capsule left, Capsule right) 
```
No Summary
## Referencing Members

```c#
PhysicsTraceBuilder = PhysicsTraceBuilder.Capsule( Capsule ) 
```
```c#
PhysicsTraceBuilder = PhysicsTraceBuilder.Capsule( Capsule, in Vector3, in Vector3 ) 
```
```c#
PhysicsTraceBuilder = PhysicsTraceBuilder.Capsule( Capsule, in Ray, in float ) 
```
```c#
Capsule = CapsulePart.Capsule { get; init; } 
```
```c#
static Trace = Trace.Capsule( Capsule, in Vector3, in Vector3 ) 
```
```c#
static Trace = Trace.Capsule( Capsule, in Ray, in float ) 
```
```c#
void GizmoDraw.LineCapsule( Capsule, int ) 
```
```c#
PhysicsGroup = ModelEntity.SetupPhysicsFromCapsule( PhysicsMotionType, Capsule ) 
```
```c#
PhysicsGroup = ModelEntity.SetupPhysicsFromCylinder( PhysicsMotionType, Capsule ) 
```
```c#
PhysicsGroup = ModelEntity.SetupPhysicsFromOrientedCapsule( PhysicsMotionType, Capsule ) 
```
