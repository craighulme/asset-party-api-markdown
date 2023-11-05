# PhysicsJoint

## 
```c#
Implements IHandle
```

## Summary

A physics constraint.
## Properties

```c#
float AngularStrength { get; set; } 
```
Strength of the angular constraint. If it takes any more energy than this, it'll break.
```c#
PhysicsBody Body1 { get; } 
```
The source physics body this joint is attached to.
```c#
PhysicsBody Body2 { get; } 
```
The target physics body this joint is constraining.
```c#
bool Collisions { get; set; } 
```
Enables or disables collisions between the 2 constrained physics bodies.
```c#
bool EnableAngularConstraint { get; set; } 
```
Enables of disables angular part of the constraint. If angular constraint is not active then objects are free to rotate (but not translate) independently.
```c#
bool EnableLinearConstraint { get; set; } 
```
Enables of disables linear part of the constraint. If linear constraint is not active then objects are free to translate (but not rotate) independently.
```c#
bool IsActive { get; } 
```
Whether this constraint is active. (i.e. is enabled, is not broken)
```c#
PhysicsPoint Point1 { get; } 
```
A specific point this joint is attached at onPhysicsJoint.Body1
```c#
PhysicsPoint Point2 { get; } 
```
A specific point this joint is attached at onPhysicsJoint.Body2
```c#
float Strength { get; set; } 
```
Strength of the linear constraint. If it takes any more energy than this, it'll break.
```c#
PhysicsWorld World { get; } 
```
TheSandbox.PhysicsWorldthis joint belongs to.
## Methods

```c#
static BallSocketJoint CreateBallSocket( PhysicsBody body1, PhysicsBody body2, Vector3 origin) 
```
Creates a ball socket constraint.
```c#
static FixedJoint CreateFixed( PhysicsPoint a, PhysicsPoint b) 
```
Creates an almost solid constraint between two physics bodies.
```c#
static HingeJoint CreateHinge( PhysicsBody body1, PhysicsBody body2, Vector3 center, Vector3 axis) 
```
Creates a hinge constraint.
```c#
static SpringJoint CreateLength( PhysicsPoint a, PhysicsPoint b, float maxLength) 
```
Creates a constraint like a rope, where it has no minimum length but its max length is restrained.
```c#
static PulleyJoint CreatePulley( PhysicsBody body1, PhysicsBody body2, Vector3 anchor1, Vector3 ground1, Vector3 anchor2, Vector3 ground2) 
```
Creates a pulley constraint, imagine it as a virtual rope connected to two objects through two anchor points.
```c#
static SliderJoint CreateSlider( PhysicsPoint a, PhysicsPoint b, float minLength, float maxLength) 
```
Creates a slider constraint between two physics bodies viaPhysics.PhysicsPoints.
```c#
static SliderJoint CreateSlider( PhysicsBody body1, PhysicsBody body2, Vector3 axis, float minLength, float maxLength) 
```
Creates a slider constraint between two physics bodies.
```c#
static SpringJoint CreateSpring( PhysicsPoint a, PhysicsPoint b, float minLength, float maxLength) 
```
Creates a constraint that will try to stay the same length, like a spring, or a rod.
```c#
void Remove( ) 
```
Removes this joint.
## Events

```c#
OnBreak( ) 
```
Called when the joint breaks.
## Inheriting Types

