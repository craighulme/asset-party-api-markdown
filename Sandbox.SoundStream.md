# SoundStream

## 
```c#
Implements IHandle
```

## Summary

Number of audio channels, as set during its creation.
## Constructors

```c#
SoundStream( int sampleRate = 44100, int channels = 1) 
```
No Summary
## Properties

```c#
int Channels { get; } 
```
Number of audio channels, as set during its creation.
```c#
int LatencySamplesCount { get; } 
```
No Summary
```c#
int MaxWriteSampleCount { get; } 
```
No Summary
```c#
int QueuedSampleCount { get; } 
```
No Summary
```c#
int SampleRate { get; } 
```
Number of samples per second, as set during its creation.
## Methods

```c#
void Delete( ) 
```
No Summary
```c#
SoundHandle Play( IEntity entity = null) 
```
Play sound of the stream. If there's already a sound playing, it will stop.
```c#
void WriteData( Span<Int16> data) 
```
No Summary
