# Triangle

## 
```c#
Implements IEquatable<Triangle>
```

## Summary

OverridesValueType.Equals
## Constructors

```c#
Triangle( Vector3 a, Vector3 b, Vector3 c) 
```
No Summary
## Fields

```c#
Vector3 A
```
No Summary
```c#
Vector3 B
```
No Summary
```c#
Vector3 C
```
No Summary
## Properties

```c#
float Area { get; } 
```
No Summary
```c#
bool IsRight { get; } 
```
No Summary
```c#
Vector3 Normal { get; } 
```
No Summary
```c#
float Perimeter { get; } 
```
No Summary
## Methods

```c#
Vector3 ClosestPoint( in Vector3 P) 
```
No Summary
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( Triangle o) 
```
OverridesValueType.Equals
```c#
override int GetHashCode( ) 
```
OverridesValueType.GetHashCode
## Operators

```c#
bool ==( Triangle left, Triangle right) 
```
No Summary
```c#
bool !=( Triangle left, Triangle right) 
```
No Summary
## Referencing Members

```c#
IEnumerable<Triangle> = MeshPart.GetTriangles( ) 
```
```c#
IEnumerable<Triangle> = Node.Triangles { get; } 
```
