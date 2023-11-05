# WorldEntity

## ```c#
Derives from ModelEntity
```

## Summary

The world entity.
## Constructors

```c#
WorldEntity( ) 
```
No Summary
## Methods

```c#
override void ClientSpawn( ) 
```
OverridesEntity.ClientSpawnCalled when the entity spawns on client.
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
