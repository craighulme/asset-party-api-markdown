# PickupTrigger

## 
```c#
Derives from ModelEntity
```

## Summary

A utility class. Add as a child to your pickupable entities to expand
the trigger boundaries. They'll be able to pick up the parent entity
using these bounds.
## Constructors

```c#
PickupTrigger( ) 
```
No Summary
## Methods

```c#
void SetTriggerSize( float radius) 
```
Set the trigger radius. Default is 16.
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
