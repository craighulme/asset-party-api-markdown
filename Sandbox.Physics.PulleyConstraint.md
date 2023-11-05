# PulleyConstraint

## ```c#
Derives from BaseConstraint
```

## Summary

A constraint that is essentially two length constraints and two points. Imagine it as a virtual rope connected to two objects, each suspended from a pulley above them.
The constraint keeps the sum of the distances between the pulley points and their suspended objects constant.
## Constructors

```c#
PulleyConstraint( ) 
```
No Summary
## Properties

```c#
Vector3 Position2 { get; set; } 
```
The position of the pulley for Entity 2.
The pulley for Entity 1 is the origin of this constraint entity.
Entity 1 is always suspended from pulley point 1, and Entity 2 is always suspended from pulley point 2.
## Methods

```c#
protected override PhysicsJoint CreateJoint( PhysicsBody body1, PhysicsBody body2) 
```
OverridesBaseConstraint.CreateJointCalled to create the joint/constraint.
```c#
protected override void DrawOverlay( ) 
```
OverridesBaseConstraint.DrawOverlayUsed to draw debug information about the joint, when it, or one of its attached entities have debug flags enabled.
