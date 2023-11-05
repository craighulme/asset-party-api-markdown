# NavPathSegment

## 
```c#
Derives from object
```

## Summary

Can this segment be optimized out
## Properties

```c#
bool AllowOptimise { get; } 
```
Can this segment be optimized out
```c#
NavArea Area { get; } 
```
The current navigation area this segment is in
```c#
float BoundaryDistance { get; } 
```
Distance to the boundary
```c#
float Curvature { get; } 
```
How much the path "curves" at this point in the XY plane (0 = none, 1 = 180 degree double-back)
```c#
float DistanceFromStart { get; } 
```
How far away is this segment to the very start of our path
```c#
Vector3 Forward { get; } 
```
The direction of the segment
```c#
NavTraverseType How { get; } 
```
How to move from one segment to the next
```c#
float Length { get; } 
```
The length of the current segment
```c#
Vector3 Position { get; } 
```
The start position of the segment
```c#
NavArea PreviousArea { get; } 
```
The previous which this segment came from
```c#
Vector3 SegmentAcceleration { get; } 
```
How much acceleration this segment has
```c#
float SegmentSpeed { get; } 
```
How much speed this segment is
```c#
NavNodeType SegmentType { get; } 
```
The type of segment this is
