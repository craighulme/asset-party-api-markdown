# CubicToPathCommand

## Derives from PathCommand
Implements IEquatable< CubicToPathCommand>

## Summary

Seehttps://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial/Paths#b%C3%A9zier_curves.
## Constructors

```c#
CubicToPathCommand( float X0, float Y0, float X1, float Y1, float X2, float Y2) 
```
Seehttps://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial/Paths#b%C3%A9zier_curves.
```c#
protected CubicToPathCommand( CubicToPathCommand original) 
```
No Summary
## Properties

```c#
float X0 { get; init; } 
```
No Summary
```c#
float X1 { get; init; } 
```
No Summary
```c#
float X2 { get; init; } 
```
No Summary
```c#
float Y0 { get; init; } 
```
No Summary
```c#
float Y1 { get; init; } 
```
No Summary
```c#
float Y2 { get; init; } 
```
No Summary
## Methods

```c#
void Deconstruct( out float X0, out float Y0, out float X1, out float Y1, out float X2, out float Y2) 
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
override bool Equals( CubicToPathCommand other) 
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
bool ==( CubicToPathCommand left, CubicToPathCommand right) 
```
ImplementsPathCommand.op_Equality
```c#
bool !=( CubicToPathCommand left, CubicToPathCommand right) 
```
ImplementsPathCommand.op_Inequality
