# WaterFunc

## 
```c#
Derives from Water
```

## Summary

Generic water volume. Make sure to have light probe volume envelop the volume of the water for the water to gain proper lighting.
## Constructors

```c#
WaterFunc( ) 
```
No Summary
## Methods

```c#
override void ClientSpawn( ) 
```
OverridesWater.ClientSpawnCalled when the entity spawns on client.
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
