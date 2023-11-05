# PushVolumeEntity

## Derives from BaseTrigger

## Summary

A volume that pushes entities that are touching it.
## Constructors

```c#
PushVolumeEntity( ) 
```
No Summary
## Properties

```c#
float Force { get; set; } 
```
How strong should we be pushing other entities
```c#
Angles ForceDirection { get; set; } 
```
Direction of the force.
```c#
bool OnlyPushOnEnter { get; set; } 
```
If set, applies 1 second worth of force only when an entity enters the trigger
## Methods

```c#
protected void SetForce( float force) 
```
Sets the force per second for this push volume
```c#
override void OnTouchStart( Entity toucher) 
```
OverridesBaseTrigger.OnTouchStartAn entity that passes PassesTriggerFilters has started touching the trigger
