# ArcToPathCommand

## Derives from PathCommand
Implements IEquatable<ArcToPathCommand>

## Summary

Seehttps://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial/Paths#arcs.
## Constructors

```c#
ArcToPathCommand( float Rx, float Ry, float XAxisRotate, PathArcSize LargeArc, PathDirection Sweep, float X, float Y) 
```
Seehttps://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial/Paths#arcs.
```c#
protected ArcToPathCommand( ArcToPathCommand original) 
```
No Summary
## Properties

```c#
PathArcSize LargeArc { get; init; } 
```
No Summary
```c#
float Rx { get; init; } 
```
No Summary
```c#
float Ry { get; init; } 
```
No Summary
```c#
PathDirection Sweep { get; init; } 
```
No Summary
```c#
float X { get; init; } 
```
No Summary
```c#
float XAxisRotate { get; init; } 
```
No Summary
```c#
float Y { get; init; } 
```
No Summary
## Methods

```c#
void Deconstruct( out float Rx, out float Ry, out float XAxisRotate, out PathArcSize LargeArc, out PathDirection Sweep, out float X, out float Y) 
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
override bool Equals( ArcToPathCommand other) 
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
bool ==( ArcToPathCommand left, ArcToPathCommand right) 
```
ImplementsPathCommand.op_Equality
```c#
bool !=( ArcToPathCommand left, ArcToPathCommand right) 
```
ImplementsPathCommand.op_Inequality
