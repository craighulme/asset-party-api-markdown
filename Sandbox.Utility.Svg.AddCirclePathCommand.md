# AddCirclePathCommand

## ```c#
Implements IEquatable<AddCirclePathCommand>
```

## Summary

Seehttps://developer.mozilla.org/en-US/docs/Web/SVG/Element/circle.
## Constructors

```c#
AddCirclePathCommand( float X, float Y, float Radius) 
```
Seehttps://developer.mozilla.org/en-US/docs/Web/SVG/Element/circle.
```c#
protected AddCirclePathCommand( AddCirclePathCommand original) 
```
No Summary
## Properties

```c#
float Radius { get; init; } 
```
No Summary
```c#
float X { get; init; } 
```
No Summary
```c#
float Y { get; init; } 
```
No Summary
## Methods

```c#
void Deconstruct( out float X, out float Y, out float Radius) 
```
No Summary
```c#
override bool Equals( object obj) 
```
OverridesPathCommand.Equals
```c#
override bool Equals( PathCommand other) 
```
OverridesPathCommand.Equals
```c#
override bool Equals( AddCirclePathCommand other) 
```
OverridesPathCommand.Equals
```c#
override int GetHashCode( ) 
```
OverridesPathCommand.GetHashCode
```c#
override string ToString( ) 
```
OverridesPathCommand.ToString
## Operators

```c#
bool ==( AddCirclePathCommand left, AddCirclePathCommand right) 
```
ImplementsPathCommand.op_Equality
```c#
bool !=( AddCirclePathCommand left, AddCirclePathCommand right) 
```
ImplementsPathCommand.op_Inequality
