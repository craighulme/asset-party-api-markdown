# PositionMode

## ```c#
Derives from Enum
```

## Summary

Possible values forpositionCSS property.
## Fields

```c#
static PositionMode Absolute = 2
```
Same asPositionMode.Relative, but the elements size does not affect other elements at all.
```c#
static PositionMode Relative = 1
```
Enablestop,right,bottom,left, andz-indexto offset the element from its
would-be position withPositionMode.Static.
```c#
static PositionMode Static = 0
```
Default, thetop,right,bottom,left, andz-indexproperties have no effect.
## Referencing Members

```c#
PositionMode? = BaseStyles.Position { get; set; } 
```
