# HandPoseAttribute

## 
```c#
Derives from BaseModelDocAttribute
```

## Summary

A helper used for VR hand purposes.
## Constructors

```c#
HandPoseAttribute( string originKey, string anglesKey, string model, bool isRightHand) 
```
No Summary
## Properties

```c#
string Enabled { get; set; } 
```
Internal name of the key that controls whether this helper is visible or not.
```c#
string Label { get; set; } 
```
Text label this helper will have when hovered/selected.
## Methods

```c#
protected override void AddKeys( Dictionary<string, object> dict) 
```
OverridesBaseModelDocAttribute.AddKeysAdd generic key-values to the helper.
