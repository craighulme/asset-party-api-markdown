# Voice

## 
```c#
Derives from object
```

## Summary

Do we want to send our microphone input to server?
## Properties

```c#
static bool Enabled { get; } 
```
Do we want to send our microphone input to server?
```c#
static bool IsRecording { get; } 
```
Returns true if your voice is actually recording. This means you're pressing your PTT key (or have always talk on)
and you're actually making noise that is being recorded and sent to other computers.
```c#
static float Level { get; } 
```
Last voice level sent to server
```c#
static bool Loopback { get; } 
```
Do we want to play back our own voice?
```c#
static int SampleRate { get; } 
```
Available clientside, this is the sample rate that we're encoding our voice at
