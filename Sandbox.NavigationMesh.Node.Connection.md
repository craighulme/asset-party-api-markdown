# Connection

## ```c#
Implements IEquatable<Connection>
```

## Summary

OverridesObject.Equals
## Constructors

```c#
Connection( Node Target, float StepHeight, Line Line) 
```
No Summary
```c#
protected Connection( Connection original) 
```
No Summary
## Properties

```c#
Line Line { get; init; } 
```
No Summary
```c#
float StepHeight { get; init; } 
```
No Summary
```c#
Node Target { get; init; } 
```
No Summary
## Methods

```c#
void Deconstruct( out Node Target, out float StepHeight, out Line Line) 
```
No Summary
```c#
override bool Equals( object obj) 
```
OverridesObject.Equals
```c#
override bool Equals( Connection other) 
```
OverridesObject.Equals
```c#
override int GetHashCode( ) 
```
OverridesObject.GetHashCode
```c#
override string ToString( ) 
```
OverridesObject.ToString
## Operators

```c#
bool ==( Connection left, Connection right) 
```
No Summary
```c#
bool !=( Connection left, Connection right) 
```
No Summary
