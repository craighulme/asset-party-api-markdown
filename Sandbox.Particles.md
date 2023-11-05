# Particles

## ```c#
Implements IDisposable
```

## Summary

A particle system.
## Constructors

```c#
Particles( ) 
```
No Summary
## Properties

```c#
bool EnableDrawing { get; set; } 
```
Should we be drawing the particles or not
```c#
bool Simulating { get; set; } 
```
Should we play the particle simulation or not
```c#
float TimeScale { get; set; } 
```
Time scale for this particle system.
## Methods

```c#
static Particles Create( string name) 
```
Create a particle system by name.
```c#
static Particles Create( string name, Vector3 position) 
```
Create a particle system by name at a world position.
```c#
static Particles Create( string name, Entity entity, bool follow = true) 
```
Create a particle system by name tied to an entity.
```c#
static Particles Create( string name, Entity entity, string attachment, bool follow = true) 
```
Create a particle system by name tied to an attachment on an entity.
```c#
virtual void Dispose( ) 
```
ImplementsIDisposable.DisposeDispose of this particle system
```c#
void Destroy( bool immediately = false) 
```
Destroy this particle system.
```c#
void Set( in string name, in float value) 
```
Set named value as a float.
```c#
void Set( in string name, in Vector3 value) 
```
Set named value as a vector.
```c#
void SetEntity( int index, Entity entity, bool follow = true) 
```
Set the control point to an entity's origin. Can specify whether to follow or not.
```c#
void SetEntity( int index, Entity entity, Vector3 offset, bool follow = true) 
```
Set the control point to an entity's origin offset by the local offset.
```c#
void SetEntityAttachment( int index, Entity entity, string attachment, bool follow = true) 
```
Set the control point to an entity's attachment position. Can specify whether to follow or not.
```c#
void SetEntityAttachment( int index, Entity entity, string attachmentName, Vector3 offset, ParticleAttachment attachment = 5) 
```
Set the control point to an entity's attachment position with an offset and custom attachment type.
```c#
void SetEntityBone( int index, Entity entity, int boneId, Transform offset = null, bool follow = true) 
```
Set the control point to an entity's bone position. Can specify whether to follow or not.
```c#
void SetForward( int index, Vector3 forward) 
```
Set control point data as a direction vector.
```c#
void SetModel( int index, Model model) 
```
Sets the model of the control point.
```c#
void SetOrientation( int index, Angles angles) 
```
Set control point data as an orientation.
```c#
void SetOrientation( int index, Rotation rotation) 
```
Set control point data as an orientation. Converts Rotation to Angles for you.
```c#
void SetPosition( int index, Vector3 position) 
```
Set control point data as a position vector.
```c#
void SetPositionComponent( int index, int component, float value) 
```
Set a single component of a given control point's position.
```c#
void SetSnapshot( int index, string assetName) 
```
Sets the particle snapshot by asset name.
```c#
void SetSnapshot( int index, ParticleSnapshot resource) 
```
Sets the particle snapshot by resource.
