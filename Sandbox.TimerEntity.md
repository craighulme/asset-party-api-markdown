# TimerEntity

## Derives from Entity

## Summary

An entity that fires a timer event at regular or random intervals.TODO: This is a stop-gap solution and may be removed in the future in favor of "map blueprints" or node based Map I/O.
## Constructors

```c#
TimerEntity( ) 
```
No Summary
## Methods

```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
