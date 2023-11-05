# NavBlockerEntity

## 
```c#
Derives from ModelEntity
```

## Summary

Has the ability to dynamically block the navigation mesh. When active, AI will see this entity as an obstacle and will not try to walk through it.
## Constructors

```c#
NavBlockerEntity( ) 
```
No Summary
## Properties

```c#
bool Enabled { get; protected set; } 
```
Enabled state of this entity.
## Methods

```c#
void Disable( ) 
```
Disables this blocker.
```c#
void Enable( ) 
```
Enables this blocker.
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
