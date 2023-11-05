# AddOvalPathCommand

## Derives from PathCommand
Implements IEquatable< AddOvalPathCommand>

## Summary

Seehttps://developer.mozilla.org/en-US/docs/Web/SVG/Element/ellipse.
## Constructors

```c#
AddOvalPathCommand( Rect Rect) 
```
Seehttps://developer.mozilla.org/en-US/docs/Web/SVG/Element/ellipse.
```c#
protected AddOvalPathCommand( AddOvalPathCommand original) 
```
No Summary
## Properties

```c#
Rect Rect { get; init; } 
```
No Summary
## Methods

```c#
void Deconstruct( out Rect Rect) 
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
override bool Equals( AddOvalPathCommand other) 
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
bool ==( AddOvalPathCommand left, AddOvalPathCommand right) 
```
ImplementsPathCommand.op_Equality
```c#
bool !=( AddOvalPathCommand left, AddOvalPathCommand right) 
```
ImplementsPathCommand.op_Inequality
