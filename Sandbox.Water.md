# Water

## ```c#
Derives from ModelEntity
```

## Summary

OverridesEntity.ClientSpawnCalled when the entity spawns on client.
## Constructors

```c#
Water( ) 
```
No Summary
## Methods

```c#
override void ClientSpawn( ) 
```
OverridesEntity.ClientSpawnCalled when the entity spawns on client.
```c#
override void EndTouch( Entity other) 
```
OverridesEntity.EndTouchAn entity has stopped touching this trigger entity. RequiresEnableTouchenabled on this entity.
```c#
protected override void OnDestroy( ) 
```
OverridesEntity.OnDestroyCalled when the entity was destroyed. This is not the same as the class destructor.
```c#
override void Simulate( IClient cl) 
```
OverridesEntity.SimulateCalled when simulating as part of a player's tick. Like if it's a pawn.
```c#
override void StartTouch( Entity other) 
```
OverridesEntity.StartTouchAn entity has started touching this trigger entity. RequiresEnableTouchenabled on this entity.For solid collisions, seeEntity.OnPhysicsCollision.
```c#
override void TakeDamage( DamageInfo info) 
```
OverridesEntity.TakeDamageCalled when the entity receives a damage event. This is where you want to subtract health, etc.
```c#
override void Touch( Entity other) 
```
OverridesEntity.TouchAn entity has touched this trigger entity. RequiresEnableTouchenabled on this entity.See alsoModelEntity.EnableTouchPersists.
## Inheriting Types

