# VoiceRecording

## ```c#
Derives from object
```

## Summary

Flush any recorded data so we don't have it kept in memory
## Methods

```c#
static void Flush( ) 
```
Flush any recorded data so we don't have it kept in memory
```c#
static bool Save( string path) 
```
Grab any recorded voice data and save it as a WAV file
```c#
static void Start( int samples = 44100, int bytesPerSecond = 192000) 
```
Start recording data from microphone
```c#
static void Stop( ) 
```
Stop recording data from microphone
