# TriggerOnce

## ```c#
Derives from BaseTrigger
```

## Summary

A simple trigger volume that fires once and then removes itself.
## Constructors

```c#
TriggerOnce( ) 
```
No Summary
## Properties

```c#
protected Output OnTrigger { get; set; } 
```
Called once at least a single entity that passes filters is touching this trigger, just before this trigger getting deleted
## Methods

```c#
protected virtual void OnTriggered( Entity other) 
```
The trigger has been... triggered. The entity passed all the filters.
```c#
override void OnTouchStart( Entity other) 
```
OverridesBaseTrigger.OnTouchStartAn entity that passes PassesTriggerFilters has started touching the trigger
```c#
override void Spawn( ) 
```
OverridesBaseTrigger.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
