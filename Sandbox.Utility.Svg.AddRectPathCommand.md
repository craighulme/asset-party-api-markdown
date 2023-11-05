# AddRectPathCommand

## 
```c#
Implements IEquatable<AddRectPathCommand>
```

## Summary

Seehttps://developer.mozilla.org/en-US/docs/Web/SVG/Element/rect.
## Constructors

```c#
AddRectPathCommand( Rect Rect) 
```
Seehttps://developer.mozilla.org/en-US/docs/Web/SVG/Element/rect.
```c#
protected AddRectPathCommand( AddRectPathCommand original) 
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
override bool Equals( AddRectPathCommand other) 
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
bool ==( AddRectPathCommand left, AddRectPathCommand right) 
```
ImplementsPathCommand.op_Equality
```c#
bool !=( AddRectPathCommand left, AddRectPathCommand right) 
```
ImplementsPathCommand.op_Inequality
