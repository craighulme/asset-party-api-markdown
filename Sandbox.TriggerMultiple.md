# TriggerMultiple

## Derives from BaseTrigger

## Summary

A volume that can be triggered multiple times, including at an interval while something is inside the trigger volume.
## Constructors

```c#
TriggerMultiple( ) 
```
No Summary
## Properties

```c#
float Cooldown { get; set; } 
```
Amount of time, in seconds, after the trigger_multiple has triggered before it can be triggered again. If set to -1, it will never trigger again (in which case you should just use a trigger_once). This affects OnTrigger output.
```c#
protected Output OnTrigger { get; set; } 
```
Called every "Delay before reset" seconds as long as at least one entity that passes filters is touching this trigger
## Methods

```c#
protected virtual void OnTriggered( Entity other) 
```
The trigger has been... triggered. The entity passed all the filters, and the timeout has passed.
```c#
override void Spawn( ) 
```
OverridesBaseTrigger.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
```c#
override void Touch( Entity other) 
```
OverridesBaseTrigger.TouchAn entity has touched this trigger entity. RequiresEnableTouchenabled on this entity.See alsoModelEntity.EnableTouchPersists.
