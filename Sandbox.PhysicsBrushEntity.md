# PhysicsBrushEntity

## Derives from BasePhysics

## Summary

A generic non model physics object.
## Constructors

```c#
PhysicsBrushEntity( ) 
```
No Summary
## Properties

```c#
protected float HealthOverride { get; set; } 
```
Amount of damage this entity can take before breaking
```c#
protected Output OnDamaged { get; set; } 
```
Fired when the entity gets damaged
```c#
string PropData { get; set; } 
```
Physical surface properties of this physics mesh.
```c#
StartAsState StartAs { get; set; } 
```
Allows disabling physics simulation, or start frozen mid air until a physics collision.
## Methods

```c#
protected void DisableMotion( ) 
```
Disable motion (gravity, etc) on this entity
```c#
protected void EnableMotion( ) 
```
Enable motion (gravity, etc) on this entity
```c#
protected void Sleep( ) 
```
Wake up this physics object, if it is sleeping.
```c#
protected void Wake( ) 
```
Wake up this physics object, if it is sleeping.
```c#
override void ClientSpawn( ) 
```
OverridesEntity.ClientSpawnCalled when the entity spawns on client.
```c#
override void Spawn( ) 
```
OverridesBasePhysics.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
```c#
override void TakeDamage( DamageInfo info) 
```
OverridesBasePhysics.TakeDamageCalled when the entity receives a damage event. This is where you want to subtract health, etc.
## Nested Types

