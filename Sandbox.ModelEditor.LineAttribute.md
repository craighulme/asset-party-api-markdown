# LineAttribute

## Derives from BaseModelDocAttribute

## Summary

Internal name of the key that dictates which attachment to use as parent for start position.
## Constructors

```c#
LineAttribute( ) 
```
No Summary
## Properties

```c#
string AttachmentFrom { get; set; } 
```
Internal name of the key that dictates which attachment to use as parent for start position.
```c#
string AttachmentTo { get; set; } 
```
Internal name of the key that dictates which attachment to use as parent for end position.
```c#
string BoneFrom { get; set; } 
```
Internal name of the key that dictates which bone to use as parent for start position.
```c#
string BoneTo { get; set; } 
```
Internal name of the key that dictates which bone to use as parent for end position.
```c#
string Color { get; set; } 
```
A string formatted color for this helper. Format is "255 255 255"
```c#
string Enabled { get; set; } 
```
Internal name of the key that controls whether this helper is visible or not.
```c#
string OriginFrom { get; set; } 
```
Internal name of the key to read line start position from.
```c#
string OriginTo { get; set; } 
```
Internal name of the key to read line end position from.
```c#
float Width { get; set; } 
```
The width of the line helper
## Methods

```c#
protected override void AddKeys( Dictionary<string, object> dict) 
```
OverridesBaseModelDocAttribute.AddKeysAdd generic key-values to the helper.
```c#
protected override void AddTransform( StringBuilder sb) 
```
OverridesBaseModelDocAttribute.AddTransformInternal, used to add multi level key-values.
