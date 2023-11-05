# SpringConstraint

## Derives from BaseConstraint

## Summary

A physically simulated spring.
'Length' is what's known as the 'natural spring length'. This is how long the spring would be if it was at rest (nothing hanging on it or attached).
When you attach something to the spring, it will stretch longer than its 'natural length'.
The amount of stretch is determined by the 'Spring Frequency'.
The larger the spring frequency the less stretch the spring.
## Constructors

```c#
SpringConstraint( ) 
```
No Summary
## Properties

```c#
float Damping { get; set; } 
```
How much energy the spring loses. Values less than one give you an oscillating spring. A value of one makes the spring return without overshooting
```c#
float Frequency { get; set; } 
```
The stiffness of the spring.  The larger the number the less the spring will stretch. The maximum should be not more than 30!
```c#
float Length { get; set; } 
```
How long the spring would be if it was at rest (nothing hanging on it or attached). 0 means the length of the helper.
```c#
Vector3 SpringAxis { get; set; } 
```
Use the helper. Drag it out to match the virtual spring.
## Methods

```c#
protected override PhysicsJoint CreateJoint( PhysicsBody body1, PhysicsBody body2) 
```
OverridesBaseConstraint.CreateJointCalled to create the joint/constraint.
```c#
protected override void DrawOverlay( ) 
```
OverridesBaseConstraint.DrawOverlayUsed to draw debug information about the joint, when it, or one of its attached entities have debug flags enabled.
