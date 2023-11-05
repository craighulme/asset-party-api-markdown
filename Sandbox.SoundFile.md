# SoundFile

## Derives from Resource
Implements IValid

## Summary

A sound resource.
## Properties

```c#
virtual bool IsValid { get; } 
```
ImplementsIValid.IsValidWhether this object is valid or not.
```c#
int BitsPerSample { get; } 
```
Bits per each sample of this sound file.
```c#
int BytesPerSample { get; } 
```
Bytes per each sample of this sound file.
```c#
int Channels { get; } 
```
Number of channels this audio file has.
```c#
float Duration { get; } 
```
Duration of the sound this sound file contains, in seconds.
```c#
SoundFormat Format { get; } 
```
Format of the audio file.
```c#
Action OnReloaded { get; set; } 
```
Ran when the file is reloaded/recompiled, etc.
```c#
int Rate { get; } 
```
Sample rate of this sound file, per second.
```c#
int SampleFrameSize { get; } 
```
Size of one sample, typically this would be "sample size * channel count", but can vary on audio format.
## Methods

```c#
static SoundFile Load( string filename) 
```
Load a new sound from disk. Includes automatic caching.
```c#
Task<Int16[]> GetSamplesAsync( ) 
```
Request decompressed audio samples.
```c#
Task<bool> LoadAsync( ) 
```
No Summary
