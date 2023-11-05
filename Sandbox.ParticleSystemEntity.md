# ParticleSystemEntity

## ```c#
Derives from Entity
```

## Summary

A entity that represents and allows control of a single particle system.
## Constructors

```c#
ParticleSystemEntity( ) 
```
No Summary
## Properties

```c#
Particles ActiveSystem { get; protected set; } 
```
The currently active particle system instance.
```c#
EntityTarget ControlPoint0 { get; set; } 
```
If set, control point 0 of the effect will be at this entity's location. (Otherwise it is at the info_particle_system origin)
```c#
EntityTarget ControlPoint1 { get; set; } 
```
If set, control point 1 of the effect will be at this entity's location.
```c#
EntityTarget ControlPoint2 { get; set; } 
```
If set, control point 2 of the effect will be at this entity's location. If control point 1 is not set, this will be ignored.
```c#
EntityTarget ControlPoint3 { get; set; } 
```
If set, control point 3 of the effect will be at this entity's location. If control point 2 is not set, this will be ignored.
```c#
EntityTarget ControlPoint4 { get; set; } 
```
If set, control point 4 of the effect will be at this entity's location. If control point 3 is not set, this will be ignored.
```c#
EntityTarget ControlPoint5 { get; set; } 
```
If set, control point 5 of the effect will be at this entity's location. If control point 4 is not set, this will be ignored.
```c#
int DataControlPoint { get; set; } 
```
What controlpoint to set data on. -1 means this is not used.
```c#
Vector3 DataControlPointValue { get; set; } 
```
Data Control Point Value to set.
```c#
bool IsActive { get; set; } 
```
Whether this particle system is active or not.
```c#
string NamedFloat { get; set; } 
```
What Named Float to set.
```c#
float NamedFloatValue { get; set; } 
```
Data to set for the Named Float value.
```c#
string NamedVector { get; set; } 
```
What Named Vector to set.
```c#
Vector3 NamedVectorValue { get; set; } 
```
Data to set for the Named Vector.
```c#
string ParticleSystemName { get; set; } 
```
The name of the particle system.
```c#
string SnapshotFile { get; set; } 
```
A particle snapshot file) to be loaded and used by this particle system. Set to Control Point 0.
```c#
bool StartActive { get; set; } 
```
Should this system start active when it enters a player's PVS?
```c#
int TintControlPoint { get; set; } 
```
What controlpoint to set color tint on. -1 means this is not used.
```c#
Color TintControlPointColor { get; set; } 
```
Set the Tint of the Particle.
## Methods

```c#
protected void DestroyImmediately( ) 
```
Destroy the particle system and remove all particles immediately.
```c#
protected void SetControlPoint( string input) 
```
Set a Control Point via format - CP: X Y Z
```c#
protected void Start( ) 
```
Tell the particle system to start emitting.
```c#
protected void Stop( ) 
```
Tell the particle system to stop emitting.
```c#
protected void StopPlayEndCap( ) 
```
Tell the particle system to stop emitting and play its End Cap Effect.
```c#
protected override void OnDestroy( ) 
```
OverridesEntity.OnDestroyCalled when the entity was destroyed. This is not the same as the class destructor.
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
