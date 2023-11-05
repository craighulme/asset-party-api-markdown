# SoundEventEntity

## ```c#
Derives from Entity
```

## Summary

Plays a sound event from a point. The point can be this entity or a specified entity's position.
## Constructors

```c#
SoundEventEntity( ) 
```
No Summary
## Properties

```c#
bool OverrideSoundParams { get; set; } 
```
Setting this to true will override default sound parameters
```c#
Sound PlayingSound { get; protected set; } 
```
The currently playing sound instance.
```c#
string SoundName { get; set; } 
```
Name of the sound to play.
```c#
float SoundPitch { get; set; } 
```
Set the pitch of the sound
```c#
float SoundVolume { get; set; } 
```
Set the volume of the sound
```c#
string SourceEntityName { get; set; } 
```
The entity to use as the origin of the sound playback. If not set, will play from this snd_event_point.
```c#
bool StartOnSpawn { get; set; } 
```
Start the sound on spawn
```c#
bool StopOnNew { get; set; } 
```
Stop the sound before starting to play it again
## Methods

```c#
void StartSound( ) 
```
Start the sound event. If an entity name is provided, the sound will originate from that entity
```c#
void StopSound( ) 
```
Stop the sound event
```c#
override void ClientSpawn( ) 
```
OverridesEntity.ClientSpawnCalled when the entity spawns on client.
```c#
protected override void OnDestroy( ) 
```
OverridesEntity.OnDestroyCalled when the entity was destroyed. This is not the same as the class destructor.
