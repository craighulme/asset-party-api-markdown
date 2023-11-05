# ClosePathCommand

## Derives from PathCommand
Implements IEquatable<ClosePathCommand>

## Summary

Seehttps://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial/Paths#line_commands.
## Constructors

```c#
protected ClosePathCommand( ClosePathCommand original) 
```
No Summary
```c#
ClosePathCommand( ) 
```
No Summary
## Methods

```c#
override bool Equals( object obj) 
```
OverridesPathCommand.Equals
```c#
override bool Equals( PathCommand other) 
```
OverridesPathCommand.Equals
```c#
override bool Equals( ClosePathCommand other) 
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
bool ==( ClosePathCommand left, ClosePathCommand right) 
```
ImplementsPathCommand.op_Equality
```c#
bool !=( ClosePathCommand left, ClosePathCommand right) 
```
ImplementsPathCommand.op_Inequality
