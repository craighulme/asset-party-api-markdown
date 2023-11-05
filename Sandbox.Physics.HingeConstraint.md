# HingeConstraint

## Derives from BaseConstraint

## Summary

A physically simulated hinge. Use the helper to define the axis of rotation.
## Constructors

```c#
HingeConstraint( ) 
```
No Summary
## Properties

```c#
Vector3 HingeAxis { get; set; } 
```
Position used to determine hinge axis, the axis being between this position and the position of the constraint entity. Use the helper to set the axis.
```c#
float HingeFriction { get; set; } 
```
Resistance/friction in the hinge. A value of 1 will hold the child object still under gravity
```c#
float InitialRotation { get; set; } 
```
No Summary
```c#
float MaxRotation { get; set; } 
```
Maximum rotation limit around hinge axis
```c#
float MinRotation { get; set; } 
```
Minimum rotation limit around hinge axis
```c#
float MotorDampingRatio { get; set; } 
```
No Summary
```c#
float MotorFrequency { get; set; } 
```
No Summary
## Methods

```c#
protected override PhysicsJoint CreateJoint( PhysicsBody body1, PhysicsBody body2) 
```
OverridesBaseConstraint.CreateJointCalled to create the joint/constraint.
