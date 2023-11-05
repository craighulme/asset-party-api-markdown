# AxisAttribute

## Derives from BaseTransformAttribute

## Summary

Draws 3 line axis visualization, which can set up to be manipulated via gizmos. You can have multiple of these.
## Constructors

```c#
AxisAttribute( ) 
```
No Summary
## Properties

```c#
string Enabled { get; set; } 
```
Internal name of a boolean key that dictates whether this helper should draw or not. If unset, will draw always.
```c#
bool ParentLine { get; set; } 
```
If set to true, when the node is selected a line will be drawn from the helper to the parent attachment/bone.
## Methods

```c#
protected override void AddKeys( Dictionary<string, object> dict) 
```
OverridesBaseModelDocAttribute.AddKeysAdd generic key-values to the helper.
