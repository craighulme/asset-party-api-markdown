# VideoPlayer

## 
```c#
Implements IDisposable, IWeakInteropHandle
```

## Summary

Enables video playback and access to the video texture and audio.
## Constructors

```c#
VideoPlayer( ) 
```
No Summary
## Properties

```c#
int Channels { get; } 
```
Number of audio channels.
```c#
float Duration { get; } 
```
Gets the total duration of the video in seconds.
```c#
bool HasAudio { get; } 
```
Does the loaded video have audio?
```c#
int Height { get; } 
```
Height of the video.
```c#
bool IsPaused { get; } 
```
Has the video been paused?
```c#
bool Muted { get; set; } 
```
The video is muted
```c#
Action OnAudioReady { get; set; } 
```
Event that is invoked when the audio stream is created and ready to use.
```c#
Action OnLoaded { get; set; } 
```
Video successfully loaded.
```c#
TextureChangedDelegate OnTextureData { get; set; } 
```
If this event is set, texture data will be provided instead of rendering to the texture.
```c#
float PlaybackTime { get; } 
```
Gets the current playback time in seconds.
```c#
bool Repeat { set; } 
```
Sets whether the video should loop when it reaches the end.
```c#
int SampleRate { get; } 
```
Audio sample rate.
```c#
Texture Texture { get; } 
```
Texture of the video frame.
```c#
int Width { get; } 
```
Width of the video.
## Methods

```c#
virtual void Dispose( ) 
```
ImplementsIDisposable.Dispose
```c#
void Pause( ) 
```
Pauses video playback.
```c#
void Play( string url) 
```
Plays a video file from a URL. If there's already a video playing, it will stop.
```c#
void Play( BaseFileSystem filesystem, string path) 
```
Plays a video file from a relative path. If there's already a video playing, it will stop.
```c#
SoundHandle PlayAudio( IEntity entity = null) 
```
Play audio of the stream. If there's already a sound playing, it will stop.
```c#
void Present( ) 
```
Present a video frame.
```c#
void Resume( ) 
```
Resumes video playback.
```c#
void Seek( float time) 
```
Sets the playback position to a specified time in the video, given in seconds.
```c#
void Stop( ) 
```
Stops video playback.
```c#
void TogglePause( ) 
```
Toggle video playback
## Nested Types

