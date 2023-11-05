# BasePhysics

## 
```c#
Derives from ModelEntity
```

## Summary

Base entity with physical properties, enables impact damage and the like
## Constructors

```c#
BasePhysics( ) 
```
No Summary
## Methods

```c#
protected virtual ModelPropData GetModelPropData( ) 
```
Returns model's prop data, or basic defaults if model specifies none.
```c#
protected void ApplyDamageForces( DamageInfo info) 
```
Applies physics forces from damage info.
```c#
protected override void OnPhysicsCollision( CollisionEventData eventData) 
```
OverridesEntity.OnPhysicsCollisionCalled when this entity collides with anything else via Physics.
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
```c#
override void TakeDamage( DamageInfo info) 
```
OverridesEntity.TakeDamageCalled when the entity receives a damage event. This is where you want to subtract health, etc.
## Inheriting Types

