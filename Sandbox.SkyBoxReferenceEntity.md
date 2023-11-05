# SkyBoxReferenceEntity

## Derives from Entity

## Summary

OverridesEntity.ClientSpawnCalled when the entity spawns on client.
## Constructors

```c#
SkyBoxReferenceEntity( ) 
```
No Summary
## Properties

```c#
static SkyBoxReferenceEntity Instance { get; } 
```
No Summary
```c#
bool FixupNames { get; set; } 
```
No Summary
```c#
string TargetMapName { get; set; } 
```
No Summary
```c#
string WorldGroupID { get; set; } 
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
