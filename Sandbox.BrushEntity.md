# BrushEntity

## Derives from ModelEntity

## Summary

A generic brush/mesh that can toggle its visibility and collisions, and can be broken.
## Constructors

```c#
BrushEntity( ) 
```
No Summary
## Properties

```c#
bool Collisions { get; set; } 
```
Whether this func_brush has collisions
```c#
bool Enabled { get; set; } 
```
Whether this func_brush is visible/active at all
```c#
protected float healthOverride { get; set; } 
```
If set to above 0, the entity will have this much health on spawn and will be breakable.
```c#
protected Output OnBreak { get; set; } 
```
Fired when the entity gets destroyed.
```c#
protected Output OnDamaged { get; set; } 
```
Fired when the entity gets damaged, even if it is unbreakable.
## Methods

```c#
void Break( ) 
```
Causes this prop to break, regardless if it is actually breakable or not. (i.e. ignores health and whether the model has gibs)
```c#
protected void Disable( ) 
```
Disable this func_brush, making it invisible and non solid
```c#
protected void DisableSolid( ) 
```
Make this func_brush non solid
```c#
protected void Enable( ) 
```
Enable this func_brush, making it visible
```c#
protected void EnableSolid( ) 
```
Make this func_brush solid
```c#
protected void Toggle( ) 
```
Toggle this func_brush
```c#
protected void ToggleSolid( ) 
```
Toggle solidity of this func_brush
```c#
override void OnKilled( ) 
```
OverridesEntity.OnKilledCalled (fromEntity.TakeDamageby default unless overridden) when there's no health left.
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
```c#
override void TakeDamage( DamageInfo info) 
```
OverridesEntity.TakeDamageCalled when the entity receives a damage event. This is where you want to subtract health, etc.
## Inheriting Types

