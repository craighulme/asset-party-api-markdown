# PhysicsPoint

## Derives from ValueType

## Summary

Used to describe a point on a physics body. This is used for things like joints where
you want to pass in just a body, or sometimes you want to pass in a body with a specific
location and rotation to attach to.
## Constructors

```c#
PhysicsPoint( PhysicsBody body, Vector3? localPosition = null, Rotation? localRotation = null) 
```
No Summary
## Fields

```c#
PhysicsBody Body
```
The physics body this point is attached to.
```c#
Vector3 LocalPosition
```
Position offset from the body's position.
```c#
Rotation LocalRotation
```
Rotation offset from the body's position.
## Properties

```c#
Transform LocalTransform { get; } 
```
A transform relative toPhysicsPoint.Body, containingPhysicsPoint.LocalPositionandPhysicsPoint.LocalRotationwith scale of 1.
```c#
Transform Transform { get; } 
```
Transform of this point in world space.
## Methods

```c#
static PhysicsPoint Local( PhysicsBody body, Vector3? localPosition = null, Rotation? localRotation = null) 
```
Describe an attachment using a position/rotation local to the body
```c#
static PhysicsPoint World( PhysicsBody body, Vector3? worldPosition = null, Rotation? worldRotation = null) 
```
Describe an attachment using a position/rotation from the world
## Operators

```c#
implicit PhysicsPoint =( PhysicsBody body) 
```
No Summary
## Referencing Members

```c#
static FixedJoint = PhysicsJoint.CreateFixed( PhysicsPoint, PhysicsPoint ) 
```
```c#
static SpringJoint = PhysicsJoint.CreateLength( PhysicsPoint, PhysicsPoint, float ) 
```
```c#
static SliderJoint = PhysicsJoint.CreateSlider( PhysicsPoint, PhysicsPoint, float, float ) 
```
```c#
static SpringJoint = PhysicsJoint.CreateSpring( PhysicsPoint, PhysicsPoint, float, float ) 
```
```c#
PhysicsPoint = PhysicsBody.LocalPoint( Vector3 ) 
```
```c#
PhysicsPoint = PhysicsBody.MassCenterPoint( ) 
```
```c#
PhysicsPoint = PhysicsJoint.Point1 { get; } 
```
```c#
PhysicsPoint = PhysicsJoint.Point2 { get; } 
```
```c#
PhysicsPoint = PhysicsBody.WorldPoint( Vector3 ) 
```
