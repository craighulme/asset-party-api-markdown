# AddPolyPathCommand

## Derives from PathCommand
Implements IEquatable< AddPolyPathCommand>

## Summary

Seehttps://developer.mozilla.org/en-US/docs/Web/SVG/Element/polyline,https://developer.mozilla.org/en-US/docs/Web/SVG/Element/polygon.
## Constructors

```c#
AddPolyPathCommand( IReadOnlyList<Vector2> Points, bool Close) 
```
Seehttps://developer.mozilla.org/en-US/docs/Web/SVG/Element/polyline,https://developer.mozilla.org/en-US/docs/Web/SVG/Element/polygon.
```c#
protected AddPolyPathCommand( AddPolyPathCommand original) 
```
No Summary
## Properties

```c#
bool Close { get; init; } 
```
No Summary
```c#
IReadOnlyList<Vector2> Points { get; init; } 
```
No Summary
## Methods

```c#
void Deconstruct( out IReadOnlyList<Vector2> Points, out bool Close) 
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
override bool Equals( AddPolyPathCommand other) 
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
bool ==( AddPolyPathCommand left, AddPolyPathCommand right) 
```
ImplementsPathCommand.op_Equality
```c#
bool !=( AddPolyPathCommand left, AddPolyPathCommand right) 
```
ImplementsPathCommand.op_Inequality
