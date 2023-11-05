# Soundscape

## ```c#
Derives from GameResource
```

## Summary

A soundscape is used for environmental ambiance of a map by playing a set of random sounds at given intervals.
## Constructors

```c#
Soundscape( ) 
```
No Summary
## Properties

```c#
List<LoopedSound> LoopedSounds { get; set; } 
```
Sounds that are played constantly on a loop.
```c#
RangedFloat MasterVolume { get; set; } 
```
All sound volumes in this soundscape will be scaled by this value.
```c#
List<StingSound> StingSounds { get; set; } 
```
Sounds that are played at intervals.
## Nested Types

