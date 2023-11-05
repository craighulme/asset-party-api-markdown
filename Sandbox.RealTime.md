# RealTime

## 
```c#
Derives from object
```

## Summary

Access to time.
## Properties

```c#
static float Delta { get; } 
```
The time delta (in seconds) between the last frame and the current (for all intents and purposes)
```c#
static double GlobalNow { get; } 
```
The number of a seconds since a set point in time. This value should match between servers and clients. If they have their timezone set correctly.
```c#
static float Now { get; } 
```
The time since game startup, in seconds.
```c#
static float SmoothDelta { get; } 
```
Like Delta but smoothed to avoid large disparities between deltas
