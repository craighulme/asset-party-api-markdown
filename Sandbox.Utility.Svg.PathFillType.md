# PathFillType

## Derives from Enum

## Summary

How to determine which sections of the path are filled.
## Fields

```c#
static PathFillType EvenOdd = 1
```
Regions that are enclosed by an odd number of paths are filled, other regions are empty.
```c#
static PathFillType Winding = 0
```
Clockwise paths are filled, counter-clockwise are empty.
## Referencing Members

```c#
PathFillType = SvgPath.FillType { get; } 
```
