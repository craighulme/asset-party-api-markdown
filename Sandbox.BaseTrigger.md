# BaseTrigger

## Derives from ModelEntity

## Summary

Entities with these tags can activate this trigger.
## Constructors

```c#
BaseTrigger( ) 
```
No Summary
## Properties

```c#
TagList ActivationTags { get; set; } 
```
Entities with these tags can activate this trigger.
```c#
bool Enabled { get; protected set; } 
```
Whether this entity is enabled or not.
```c#
protected Output OnEndTouch { get; set; } 
```
Fired when an entity stops touching this trigger. Only entities that passed this trigger's filters will cause this output to fire.
```c#
protected Output OnEndTouchAll { get; set; } 
```
Fired when all entities touching this trigger have stopped touching it.
```c#
protected Output OnStartTouch { get; set; } 
```
Fired when an entity starts touching this trigger. The touching entity must pass this trigger's filters to cause this output to fire.
```c#
protected Output OnStartTouchAll { get; set; } 
```
Fired when an entity starts touching this trigger while no other passing entities are touching it.
```c#
IEnumerable<Entity> TouchingEntities { get; } 
```
List of entities currently within this trigger's bounds.
```c#
int TouchingEntityCount { get; } 
```
A convenience property containing number of entities currently within this trigger's bounds.
## Methods

```c#
virtual void OnTouchEnd( Entity toucher) 
```
An entity that started touching this trigger has stopped touching
```c#
virtual void OnTouchEndAll( Entity toucher) 
```
Called when all entities touching this trigger have stopped touching it.
```c#
virtual void OnTouchStart( Entity toucher) 
```
An entity that passes PassesTriggerFilters has started touching the trigger
```c#
virtual void OnTouchStartAll( Entity toucher) 
```
Called when an entity starts touching this trigger while no other passing entities are touching it
```c#
virtual bool PassesTriggerFilters( Entity other) 
```
Determine if an entity should be allowed to touch this trigger
```c#
void Disable( ) 
```
Disables this trigger
```c#
void Enable( ) 
```
Enables this trigger
```c#
void Toggle( ) 
```
Toggles this trigger between enabled and disabled states
```c#
override void EndTouch( Entity other) 
```
OverridesEntity.EndTouchAn entity has stopped touching this trigger entity. RequiresEnableTouchenabled on this entity.
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
```c#
override void StartTouch( Entity other) 
```
OverridesEntity.StartTouchAn entity has started touching this trigger entity. RequiresEnableTouchenabled on this entity.For solid collisions, seeEntity.OnPhysicsCollision.
```c#
override void Touch( Entity other) 
```
OverridesEntity.TouchAn entity has touched this trigger entity. RequiresEnableTouchenabled on this entity.See alsoModelEntity.EnableTouchPersists.
## Inheriting Types

