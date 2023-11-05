# SoundHandle

## ```c#
Derives from ValueType
```

## Summary

Returned byAudioSystem.Play
## Properties

```c#
float ElapsedTime { get; } 
```
No Summary
```c#
bool IsPlaying { get; } 
```
Whether the sound is currently playing or not.
```c#
bool IsStopped { get; } 
```
True if the sound has been stopped
```c#
bool ListenLocal { set; } 
```
Place the listener at 0,0,0 facing 1,0,0.
```c#
Vector3 Position { set; } 
```
Position of the sound.
```c#
float Volume { get; set; } 
```
Directly change the volume of this sound
## Methods

```c#
void SetSoundFile( SoundFile name) 
```
No Summary
```c#
void Stop( bool immediate) 
```
No Summary
## Referencing Members

```c#
SoundHandle = SoundStream.Play( IEntity ) 
```
```c#
SoundHandle = AudioSystem.Play( string ) 
```
```c#
SoundHandle = AudioSystem.Play( string, IEntity ) 
```
```c#
SoundHandle = AudioSystem.Play( SoundEvent, IEntity ) 
```
```c#
SoundHandle = VideoPlayer.PlayAudio( IEntity ) 
```
