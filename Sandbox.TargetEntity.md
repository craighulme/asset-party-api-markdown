# TargetEntity

## 
```c#
Derives from Entity
```

## Summary

An entity that does nothing. Very useful as a positioning entity for other entities to refer to (i.e. the endpoint of a rope in a info_particle_system)
## Constructors

```c#
TargetEntity( ) 
```
No Summary
## Methods

```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
