# ColorFrame

## Derives from ValueType

## Summary

Keyframes times and values should range between 0 and 1
## Constructors

```c#
ColorFrame( float timedelta, Color color) 
```
No Summary
## Properties

```c#
float Time { get; set; } 
```
No Summary
```c#
Color Value { get; set; } 
```
No Summary
## Referencing Members

```c#
ImmutableList<ColorFrame> = Gradient.Colors { get; set; } 
```
```c#
ColorFrame = Gradient.Item[ int index, ] { get; set; } 
```
```c#
Gradient = Gradient.WithFrames( ImmutableList<ColorFrame> ) 
```
