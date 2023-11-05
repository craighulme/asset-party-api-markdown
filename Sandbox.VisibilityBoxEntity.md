# VisibilityBoxEntity

## ```c#
Derives from Entity
```

## Summary

A dynamic visibility culling box which can be used to hide objects at runtime and can be toggled on and off by entity I/O.
## Constructors

```c#
VisibilityBoxEntity( ) 
```
No Summary
## Properties

```c#
Vector3 BoxSize { get; set; } 
```
Size of the culling box.
```c#
Mode CullMode { get; set; } 
```
Should the box hide objects inside or outside of its bounds. If inside is selected,
any objects fully inside the box will be hidden.
If outside is selected, all active visibility boxes are considered,
and objects not intersecting any visibility boxes will be hidden.
```c#
bool Enabled { get; set; } 
```
Enable or disable the culling box.
```c#
bool StartDisabled { get; set; } 
```
Is the culling box disabled by default.
## Methods

```c#
override void ClientSpawn( ) 
```
OverridesEntity.ClientSpawnCalled when the entity spawns on client.
```c#
protected override void OnDestroy( ) 
```
OverridesEntity.OnDestroyCalled when the entity was destroyed. This is not the same as the class destructor.
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
## Nested Types

