# PhysicsTraceResult

## Derives from ValueType

## Summary

The physics object that was hit, if any
## Fields

```c#
PhysicsBody Body
```
The physics object that was hit, if any
```c#
int Bone
```
The id of the hit bone (either from hitbox or physics shape)
```c#
Vector3 Direction
```
The direction of the trace ray
```c#
Vector3 EndPosition
```
The end or hit position of the trace
```c#
float Fraction
```
A fraction [0..1] of where the trace hit between the start and the original end positions
```c#
bool Hit
```
Whether the trace hit something or not
```c#
Vector3 HitPosition
```
The hit position of the trace
```c#
Vector3 Normal
```
The hit surface normal (direction vector)
```c#
PhysicsShape Shape
```
The physics shape that was hit, if any
```c#
bool StartedSolid
```
Whether the trace started in a solid
```c#
Vector3 StartPosition
```
The start position of the trace
```c#
Surface Surface
```
The physical properties of the hit surface
```c#
string[] Tags
```
The tags that the hit shape had
```c#
int Triangle
```
The triangle index hit, if we hit a meshphysics shape
## Properties

```c#
float Distance { get; } 
```
The distance between start and end positions.
## Referencing Members

```c#
PhysicsTraceResult = PhysicsTraceBuilder.Run( ) 
```
