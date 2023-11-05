# NavPath

## ```c#
Derives from object
```

## Summary

The age since the path was constructed
## Properties

```c#
TimeSince Age { get; } 
```
The age since the path was constructed
```c#
int Count { get; } 
```
Return the amount of segments the path has
```c#
List<NavPathSegment> Segments { get; } 
```
Return all of our segments
```c#
float TotalLength { get; } 
```
The total length/distance of the entire path from start to end
