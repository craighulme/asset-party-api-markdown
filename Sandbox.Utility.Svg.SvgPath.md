# SvgPath

## Derives from object

## Summary

A shape in aSvg.SvgDocument, described as a vector path.
## Properties

```c#
Rect Bounds { get; } 
```
Enclosing bounding box for this path.
```c#
IReadOnlyList<PathCommand> Commands { get; } 
```
Description of how the path is constructed out of basic elements.
```c#
Color? FillColor { get; } 
```
Optional fill color for this path.
```c#
PathFillType FillType { get; } 
```
How to determine which sections of the path are filled.
```c#
bool IsEmpty { get; } 
```
If true, this path has no commands.
```c#
Color? StrokeColor { get; } 
```
Optional outline color for this path.
