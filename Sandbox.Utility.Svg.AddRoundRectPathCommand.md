# AddRoundRectPathCommand

## Derives from PathCommand
Implements IEquatable< AddRoundRectPathCommand>

## Summary

Seehttps://developer.mozilla.org/en-US/docs/Web/SVG/Element/rect.
## Constructors

```c#
AddRoundRectPathCommand( Rect Rect, float Rx, float Ry) 
```
Seehttps://developer.mozilla.org/en-US/docs/Web/SVG/Element/rect.
```c#
protected AddRoundRectPathCommand( AddRoundRectPathCommand original) 
```
No Summary
## Properties

```c#
Rect Rect { get; init; } 
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
## Methods

```c#
void Deconstruct( out Rect Rect, out float Rx, out float Ry) 
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
override bool Equals( AddRoundRectPathCommand other) 
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
bool ==( AddRoundRectPathCommand left, AddRoundRectPathCommand right) 
```
ImplementsPathCommand.op_Equality
```c#
bool !=( AddRoundRectPathCommand left, AddRoundRectPathCommand right) 
```
ImplementsPathCommand.op_Inequality
