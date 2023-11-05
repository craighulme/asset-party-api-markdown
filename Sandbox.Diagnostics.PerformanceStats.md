# PerformanceStats

## 
```c#
Derives from object
```

## Summary

Approximate working set of this process.
## Properties

```c#
static ulong ApproximateProcessMemoryUsage { get; } 
```
Approximate working set of this process.
```c#
static long BytesAllocated { get; } 
```
The number of bytes that were allocated on the managed heap in the last frame.
This may not include allocations from threads other than the game thread.
```c#
static double FrameTime { get; } 
```
Get the time taken, in seconds, that were required to process the previous frame.
```c#
static int Gen0Collections { get; } 
```
Number of generation 0 (fastest) garbage collections were done in the last frame.
```c#
static int Gen1Collections { get; } 
```
Number of generation 1 (fast) garbage collections were done in the last frame.
```c#
static int Gen2Collections { get; } 
```
Number of generation 2 (slow) garbage collections were done in the last frame.
```c#
static Block LastSecond { get; } 
```
Performance statistics over the last period, which is dictated by "perf_time" console command.
```c#
static float perf_time { get; set; } 
```
Update interval forPerformanceStats.LastSecond.
## Nested Types

