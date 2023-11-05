# Sound

## Derives from ValueType

## Summary

Allows playback and modification of sounds during playback.
## Properties

```c#
static Transform? Listener { get; set; } 
```
Set an override for the position and rotation of the local client's audio listener
```c#
float ElapsedTime { get; } 
```
Return the elapsed time from the start of the sound in seconds
```c#
bool Finished { get; } 
```
No Summary
```c#
bool IsPlaying { get; } 
```
Returns if a sound is currently playing
## Methods

```c#
static Sound FromEntity( To toTarget, string name, Entity entity) 
```
Create a sound originating from an entity.
```c#
static Sound FromEntity( string name, Entity entity) 
```
Create a sound originating from an entity.
```c#
static Sound FromEntity( To toTarget, string name, Entity entity, string attachment) 
```
Create a sound originating from an entity attachment.
```c#
static Sound FromEntity( string name, Entity entity, string attachment) 
```
Create a sound originating from an entity attachment.
```c#
static Sound FromScreen( To toTarget, string name, float x = 0.5, float y = 0.5) 
```
Create a sound originating from screen coordinates
```c#
static Sound FromScreen( string name, float x = 0.5, float y = 0.5) 
```
Create a sound originating from screen coordinates
```c#
static Sound FromWorld( To toTarget, string name, Vector3 position) 
```
Create a sound originating from a world position
```c#
static Sound FromWorld( string name, Vector3 position) 
```
Create a sound originating from a world position
```c#
SoundStream CreateStream( int sampleRate = 44100, int channels = 1) 
```
No Summary
```c#
Sound SetPitch( To toTarget, float pitch) 
```
Set pitch value (Note: this is always executed and is multiplied with the initial random pitch)
```c#
Sound SetPitch( float pitch) 
```
Set pitch value (Note: this is always executed and is multiplied with the initial random pitch)
```c#
Sound SetPosition( To toTarget, Vector3 position) 
```
Set the world position that this sounds originates from.
```c#
Sound SetPosition( Vector3 position) 
```
Set the world position that this sounds originates from.
```c#
Sound SetRandomPitch( To toTarget, float min, float max) 
```
Set random pitch value between min and max (Note: this is executed once)
```c#
Sound SetRandomPitch( float min, float max) 
```
Set random pitch value between min and max (Note: this is executed once)
```c#
Sound SetVolume( To toTarget, float volume) 
```
Set the volume of the sound.
```c#
Sound SetVolume( float volume) 
```
Set the volume of the sound.
```c#
Sound Stop( To toTarget) 
```
Stop the sound from playing
```c#
Sound Stop( ) 
```
Stop the sound from playing
## Referencing Members

```c#
Sound = SoundEventEntity.PlayingSound { get; protected set; } 
```
```c#
Sound = Entity.PlaySound( string ) 
```
```c#
virtual Sound = Entity.PlaySound( string, string ) 
```
```c#
override Sound = BaseViewModel.PlaySound( string, string ) 
```
```c#
override Sound = BaseWeapon.PlaySound( string, string ) 
```
