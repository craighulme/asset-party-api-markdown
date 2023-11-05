# SlideConstraint

## 
```c#
Derives from BaseConstraint
```

## Summary

A constraint that constrains an entity along a line segment.
## Constructors

```c#
SlideConstraint( ) 
```
No Summary
## Properties

```c#
bool EnableAngularConstraint { get; set; } 
```
No Summary
```c#
bool EnableLinearConstraint { get; set; } 
```
No Summary
```c#
float InitialOffset { get; set; } 
```
No Summary
```c#
bool LimitEndPoint { get; set; } 
```
Stop at the end point
```c#
float MotorDampingRatio { get; set; } 
```
No Summary
```c#
float MotorFrequency { get; set; } 
```
No Summary
```c#
float MotorMaxForceMultiplier { get; set; } 
```
No Summary
```c#
Vector3 SlideAxis { get; set; } 
```
Position used to determine sliding axis, the axis being between this position and the position of the constraint entity. Use the helper to set the axis.
```c#
float SlideFriction { get; set; } 
```
Set motor friction, 0 = no friction, 1 = friction that is about enough to counter gravity
```c#
bool UseEntityPivot { get; set; } 
```
Force joint position as constraint pivot
## Methods

```c#
protected override PhysicsJoint CreateJoint( PhysicsBody body1, PhysicsBody body2) 
```
OverridesBaseConstraint.CreateJointCalled to create the joint/constraint.
```c#
protected override void DrawOverlay( ) 
```
OverridesBaseConstraint.DrawOverlayUsed to draw debug information about the joint, when it, or one of its attached entities have debug flags enabled.
