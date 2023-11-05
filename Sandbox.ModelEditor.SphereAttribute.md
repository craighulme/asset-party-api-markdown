# SphereAttribute

## ```c#
Derives from BaseTransformAttribute
```

## Summary

Draws a sphere, which can be manipulated via gizmos. You can have multiple of these.
## Constructors

```c#
SphereAttribute( string radiusKey, string centerKey = "") 
```
No Summary
## Properties

```c#
bool HideSurface { get; set; } 
```
If set, the semi-transparent sphere "wall"/surface will not be drawn.
## Methods

```c#
protected override void AddKeys( Dictionary<string, object> dict) 
```
OverridesBaseModelDocAttribute.AddKeysAdd generic key-values to the helper.
