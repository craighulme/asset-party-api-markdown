# BaseConstraint

## Is abstract
Derives from Entity

## Summary

The internal joint of this constraint entity.
## Constructors

```c#
protected BaseConstraint( ) 
```
No Summary
## Fields

```c#
protected PhysicsJoint Joint
```
The internal joint of this constraint entity.
## Properties

```c#
string BreakSound { get; set; } 
```
A sound played when the constraint is broken.
```c#
bool EnableCollision { get; set; } 
```
Constraints disable collision between the attached entities. In some rare cases we want to enable this collision.
```c#
Entity Entity1 { get; } 
```
Source entity instance of the joint, if any. This is set automatically post spawn.
```c#
Entity Entity2 { get; } 
```
Target entity instance of the joint, if any. This is set automatically post spawn.
```c#
EntityTarget EntityName1 { get; set; } 
```
The source entity to constrain from. Leave empty to constrain from the world entity.
```c#
EntityTarget EntityName2 { get; set; } 
```
The entity we constrain to.
```c#
float ForceLimit { get; set; } 
```
The amount of impulse an impact must apply to the constraint to break it. A way of calculating this is to set it to the mass of an object that would break this constraint if it were resting on the constrained objects.
```c#
protected Output OnBreak { get; set; } 
```
Fired when the constraint breaks due to exceeding force limits or the Break input.
```c#
float TorqueLimit { get; set; } 
```
The amount of angular impulse required to break the constraint. A way of calculating this is to multiply any reference mass by the resting distance (from the center of mass of the object) needed to break the constraint.
## Methods

```c#
protected abstract PhysicsJoint CreateJoint( PhysicsBody body1, PhysicsBody body2) 
```
Called to create the joint/constraint.
```c#
protected virtual void DrawOverlay( ) 
```
Used to draw debug information about the joint, when it, or one of its attached entities have debug flags enabled.
```c#
void Break( ) 
```
Breaks the constraint.
```c#
protected override void OnDestroy( ) 
```
OverridesEntity.OnDestroyCalled when the entity was destroyed. This is not the same as the class destructor.
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
## Inheriting Types

