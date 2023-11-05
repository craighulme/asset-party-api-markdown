# MoveToPathCommand

## Derives from PathCommand
Implements IEquatable< MoveToPathCommand>

## Summary

Seehttps://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial/Paths#line_commands.
## Constructors

```c#
MoveToPathCommand( float X, float Y) 
```
Seehttps://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial/Paths#line_commands.
```c#
protected MoveToPathCommand( MoveToPathCommand original) 
```
No Summary
## Properties

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
void Deconstruct( out float X, out float Y) 
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
override bool Equals( MoveToPathCommand other) 
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
bool ==( MoveToPathCommand left, MoveToPathCommand right) 
```
ImplementsPathCommand.op_Equality
```c#
bool !=( MoveToPathCommand left, MoveToPathCommand right) 
```
ImplementsPathCommand.op_Inequality
