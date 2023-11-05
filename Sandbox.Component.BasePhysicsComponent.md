# BasePhysicsComponent

## ```c#
Derives from EntityComponent
```

## Summary

Whether gravity is enabled or not for this entity's physics bodies.
## Constructors

```c#
protected BasePhysicsComponent( ) 
```
No Summary
## Properties

```c#
bool GravityEnabled { get; set; } 
```
Whether gravity is enabled or not for this entity's physics bodies.
```c#
float GravityScale { get; set; } 
```
Scale of the gravity for this entity's physics bodies.
```c#
bool Keyframe { get; set; } 
```
If set, the physics bodies of the entity will be set to Keyframed, i.e. it will not simulate gravity.
```c#
PhysicsGroup PhysicsGroup { get; set; } 
```
The physics group that has the entity's bodies that we update viaBasePhysicsComponent.UpdateBodies.
```c#
bool StartAsleep { get; set; } 
```
If set, the physics bodies of the entity will not move until a physics collision occurs.
## Methods

```c#
protected virtual void UpdateBodies( ) 
```
Update all of the physics bodies with the latest settings.
```c#
protected virtual void UpdateBody( PhysicsBody body) 
```
Update this body with the latest settings
```c#
protected override void OnDeactivate( ) 
```
OverridesEntityComponent.OnDeactivateCalled when this component is disabled (or removed from the entity)
## Inheriting Types

