# BoxAttribute

## Derives from BaseTransformAttribute

## Summary

Draws a box, which can be manipulated via gizmos. You can have multiple of these.
## Constructors

```c#
BoxAttribute( string dimensionsKey) 
```
Store the box's dimensions in a single key, acting as (maxs-mins) which assumes the box's center is at the models origin.
The box's center can be set up to be movable via "Origin" property and rotatable via "Angles" property.
```c#
BoxAttribute( string minsKey, string maxsKey) 
```
Store the box's dimensions in 2 keys as Mins and Maxs. This type cannot be rotated.
## Properties

```c#
bool HideSurface { get; set; } 
```
If set, the semi-transparent box "walls" will not be drawn.
```c#
bool ShowGizmos { get; set; } 
```
If set, gizmos will be shown in transform mode to quickly move/scale the box.
For "dimensions" box Origin/Angles must be set.
## Methods

```c#
protected override void AddKeys( Dictionary<string, object> dict) 
```
OverridesBaseModelDocAttribute.AddKeysAdd generic key-values to the helper.
