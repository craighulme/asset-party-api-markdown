# HurtVolumeEntity

## Derives from BaseTrigger

## Summary

A trigger volume that damages entities that touch it.
## Constructors

```c#
HurtVolumeEntity( ) 
```
No Summary
## Properties

```c#
float Damage { get; set; } 
```
Amount of damage to deal to touching entities per second.
```c#
protected Output OnHurt { get; set; } 
```
Fired when anything BUT a player gets hurt by this trigger
```c#
protected Output OnHurtPlayer { get; set; } 
```
Fired when a player gets hurt by this trigger
## Methods

```c#
protected virtual void DealDamagePerTick( ) 
```
Called every server tick to deal damage to touching entities.
```c#
protected void SetDamage( float damage) 
```
Sets the damage per second for this trigger_hurt
