# Time

## 
```c#
Derives from object
```

## Summary

The delta between the last frame and the current (for all intents and purposes)
## Constructors

```c#
Time( ) 
```
No Summary
## Properties

```c#
static float Delta { get; set; } 
```
The delta between the last frame and the current (for all intents and purposes)
```c#
static float Now { get; set; } 
```
The time since game startup
```c#
static double Sound { get; } 
```
Gets the current DSP time
```c#
static double SoundDelta { get; } 
```
Gets the current delta between two DSP frames
```c#
static int Tick { get; set; } 
```
The current tick number that is being simulated.
