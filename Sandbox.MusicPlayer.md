# MusicPlayer

## ```c#
Implements IDisposable, IWeakInteropHandle
```

## Summary

Enables music playback. Use this for music, not for playing game sounds.
## Properties

```c#
float Amplitude { get; } 
```
Approximate measure of audio loudness.
```c#
int Channels { get; } 
```
Number of channels of the audio being played.
```c#
float DistanceMax { get; set; } 
```
Maximum distance this music would be audible at.
```c#
float DistanceMin { get; set; } 
```
Minimum distance this music would be audible at full volume.
```c#
float Duration { get; } 
```
Gets the total duration of the video in seconds.
```c#
IEntity Entity { get; set; } 
```
Play the audio from this entity.
```c#
bool ListenLocal { get; set; } 
```
Place the listener at 0,0,0 facing 1,0,0.
```c#
Action OnFinished { get; set; } 
```
Invoked when the audio has finished playing.
```c#
Action OnRepeated { get; set; } 
```
Invoked when the audio has repeated.
```c#
bool Paused { get; set; } 
```
Pause playback of audio.
```c#
float PlaybackTime { get; } 
```
Gets the current playback time in seconds.
```c#
Vector3 Position { get; set; } 
```
Position of the sound.
```c#
bool Repeat { get; set; } 
```
Audio will repeat when reaching the end.
```c#
int SampleRate { get; } 
```
Sample rate of the audio being played.
```c#
ReadOnlySpan<float> Spectrum { get; } 
```
1024 FFT magnitudes used for audio visualization.
```c#
string Title { get; } 
```
Get title of the track.
```c#
float Volume { get; set; } 
```
Change the volume of this music.
## Methods

```c#
static MusicPlayer Play( BaseFileSystem filesystem, string path) 
```
Plays a music file from a relative path.
```c#
static MusicPlayer PlayUrl( string url) 
```
Plays a music stream from a URL.
```c#
virtual void Dispose( ) 
```
ImplementsIDisposable.Dispose
```c#
void Seek( float time) 
```
Sets the playback position to a specified time in the audio, given in seconds.
```c#
void Stop( ) 
```
Stops audio playback.
