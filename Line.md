# Line

## ```c#
Implements IEquatable<Line>
```

## Summary

Represents a line in 3D space.
## Constructors

```c#
Line( Vector3 a, Vector3 b) 
```
No Summary
```c#
Line( Vector3 origin, Vector3 direction, float length) 
```
No Summary
## Fields

```c#
Vector3 a
```
Start position of the line.
```c#
Vector3 b
```
Start position of the line.
## Properties

```c#
Vector3 Center { get; } 
```
Returns the midpoint between a and b
```c#
Vector3 Delta { get; } 
```
Returns the result of b - a
```c#
Vector3 End { get; } 
```
End position of the line.
```c#
Vector3 Start { get; } 
```
Start position of the line.
## Methods

```c#
Vector3 ClosestPoint( in Vector3 pos) 
```
Returns closest point on this line to the given point.
```c#
bool ClosestPoint( in Ray ray, out Vector3 point_on_line) 
```
Returns closest point on this line to the given ray.
```c#
bool ClosestPoint( in Ray ray, out Vector3 point_on_line, out Vector3 point_on_ray) 
```
Returns closest point on this line to the given ray.
```c#
float Distance( Vector3 pos) 
```
Returns closest distance from this line to given point.
```c#
float Distance( Vector3 pos, out Vector3 closestPoint) 
```
Returns closest distance from this line to given point.
```c#
float SqrDistance( Vector3 pos) 
```
Returns closest squared distance from this line to given point.
```c#
bool Trace( in Ray ray, float radius, float maxDistance = 3.4028235E+38) 
```
Perform a "trace" between this line and given ray. If the 2 lines intersect, returns true.
```c#
override bool Equals( Line other) 
```
OverridesValueType.Equals
## Referencing Members

```c#
Connection.Connection( Node, float, Line ) 
```
```c#
IEnumerable<Line> = HullPart.GetLines( ) 
```
```c#
Line = Connection.Line { get; init; } 
```
