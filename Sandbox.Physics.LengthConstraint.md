# LengthConstraint

## 
```c#
Derives from BaseConstraint
```

## Summary

A constraint that preserves the distance between two entities. If the 'Keep Rigid' flag is set, think of it as a rod. If not, think off it as a virtual rope.
## Constructors

```c#
LengthConstraint( ) 
```
No Summary
## Properties

```c#
float AddLength { get; set; } 
```
Add (or subtract) this amount to the rest length of the rope.
```c#
Vector3 AttachPoint { get; set; } 
```
The position the rope attaches to object 2
```c#
bool KeepRigid { get; set; } 
```
Keep the constraint rigid, as if it were a stick.
```c#
float MinLength { get; set; } 
```
If the constraint is not rigid, this is the minimum length it can be.
```c#
string ParticleEffect { get; set; } 
```
If give, will spawn given particle as the rope. Particle's Control Point 1 will be set to the target entity, and will be removed if the constraint breaks.
## Methods

```c#
protected override PhysicsJoint CreateJoint( PhysicsBody body1, PhysicsBody body2) 
```
OverridesBaseConstraint.CreateJointCalled to create the joint/constraint.
```c#
protected override void DrawOverlay( ) 
```
OverridesBaseConstraint.DrawOverlayUsed to draw debug information about the joint, when it, or one of its attached entities have debug flags enabled.
```c#
protected override void OnDestroy( ) 
```
OverridesBaseConstraint.OnDestroyCalled when the entity was destroyed. This is not the same as the class destructor.
