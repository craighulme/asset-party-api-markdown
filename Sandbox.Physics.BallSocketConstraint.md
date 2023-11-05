# BallSocketConstraint

## 
```c#
Derives from BaseConstraint
```

## Summary

A constraint that keeps the position of two objects fixed, relative to the constraint's origin. It does not affect rotation.
## Constructors

```c#
BallSocketConstraint( ) 
```
No Summary
## Properties

```c#
float Friction { get; set; } 
```
Resistance/friction in the constraint.
## Methods

```c#
protected override PhysicsJoint CreateJoint( PhysicsBody body1, PhysicsBody body2) 
```
OverridesBaseConstraint.CreateJointCalled to create the joint/constraint.
