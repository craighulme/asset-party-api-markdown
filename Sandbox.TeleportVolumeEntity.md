# TeleportVolumeEntity

## 
```c#
Derives from BaseTrigger
```

## Summary

A simple trigger volume that teleports entities that touch it.
## Constructors

```c#
TeleportVolumeEntity( ) 
```
No Summary
## Properties

```c#
bool KeepVelocity { get; set; } 
```
If set, the teleported entity will not have it's velocity reset to 0.
```c#
protected Output OnTriggered { get; set; } 
```
Fired when the trigger teleports an entity
```c#
EntityTarget TargetEntity { get; set; } 
```
The entity specifying a location to which entities should be teleported to.
```c#
bool TeleportRelative { get; set; } 
```
If set, teleports the entity with an offset depending on where the entity was in the trigger teleport. Think world portals. Place the target entity accordingly.
## Methods

```c#
void SetRemoteDestination( string target) 
```
Set the target to teleport entities to.
```c#
override void OnTouchStart( Entity other) 
```
OverridesBaseTrigger.OnTouchStartAn entity that passes PassesTriggerFilters has started touching the trigger
