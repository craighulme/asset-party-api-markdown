# SkyCameraEntity

## ```c#
Derives from Entity
```

## Summary

An entity used to control the 3D Skybox.
Its origin is used to determine the 3D Skybox's position relative to the map.
Place this entity, in the 3D Skybox, at the point where the origin of the map should be.
## Constructors

```c#
SkyCameraEntity( ) 
```
No Summary
## Properties

```c#
static SkyCameraEntity Instance { get; } 
```
No Summary
```c#
float SkyboxScale { get; set; } 
```
Scale of the skybox.
## Methods

```c#
override void BuildNetworkTable( NetworkTable table) 
```
OverridesEntity.BuildNetworkTableThis method is overridden by codegen to make certain network features like[Net]functional. It is not meant to be used directly unless you know what you are doing.
```c#
override void ClientSpawn( ) 
```
OverridesEntity.ClientSpawnCalled when the entity spawns on client.
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
