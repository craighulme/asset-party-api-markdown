# PostProcessingVolume

## 
```c#
Derives from PostProcessingEntity
```

## Summary

Applies given post processing effect to players inside this volume.
Takes priority overpost_processing_entityfor all players inside.
For instances of overlapping volumes, last entered volume will take priority.
## Constructors

```c#
PostProcessingVolume( ) 
```
No Summary
## Methods

```c#
override void ClientSpawn( ) 
```
OverridesPostProcessingEntity.ClientSpawnCalled when the entity spawns on client.
```c#
override void EndTouch( Entity other) 
```
OverridesEntity.EndTouchAn entity has stopped touching this trigger entity. RequiresEnableTouchenabled on this entity.
```c#
override void Spawn( ) 
```
OverridesPostProcessingEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
```c#
override void StartTouch( Entity other) 
```
OverridesEntity.StartTouchAn entity has started touching this trigger entity. RequiresEnableTouchenabled on this entity.For solid collisions, seeEntity.OnPhysicsCollision.
```c#
override void Touch( Entity other) 
```
OverridesEntity.TouchAn entity has touched this trigger entity. RequiresEnableTouchenabled on this entity.See alsoModelEntity.EnableTouchPersists.
