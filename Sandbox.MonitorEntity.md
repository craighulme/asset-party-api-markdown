# MonitorEntity

## Derives from BrushEntity

## Summary

A monitor that renders the view from a givenpoint_cameraentity.
This entity requires a material with $MonitorTexture dynamic expression on one of its textures, usually "Color", to function properly.
## Constructors

```c#
MonitorEntity( ) 
```
No Summary
## Properties

```c#
EntityTarget CameraName { get; set; } 
```
Name of apoint_camerato display.
```c#
CameraEntity TargetCamera { get; set; } 
```
The camera instance currently being displayed.
## Methods

```c#
void SetCamera( string entityName) 
```
Set a new camera to display by itsname.
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
OverridesBrushEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
