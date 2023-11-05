# PhysicsIntersection

## 
```c#
Implements IEquatable<PhysicsIntersection>
```

## Summary

OverridesValueType.Equals
## Constructors

```c#
PhysicsIntersection( Target Self, Target Other, PhysicsContact Contact) 
```
No Summary
## Properties

```c#
PhysicsContact Contact { get; init; } 
```
No Summary
```c#
Target Other { get; init; } 
```
No Summary
```c#
Target Self { get; init; } 
```
No Summary
## Methods

```c#
void Deconstruct( out Target Self, out Target Other, out PhysicsContact Contact) 
```
No Summary
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( PhysicsIntersection other) 
```
OverridesValueType.Equals
```c#
override int GetHashCode( ) 
```
OverridesValueType.GetHashCode
```c#
override string ToString( ) 
```
OverridesValueType.ToString
## Operators

```c#
bool ==( PhysicsIntersection left, PhysicsIntersection right) 
```
No Summary
```c#
bool !=( PhysicsIntersection left, PhysicsIntersection right) 
```
No Summary
## Referencing Members

```c#
Action<PhysicsIntersection> = PhysicsBody.OnIntersectionStart { get; set; } 
```
```c#
Action<PhysicsIntersection> = PhysicsBody.OnIntersectionUpdate { get; set; } 
```
