# BaseTransformAttribute

## ```c#
Derives from BaseModelDocAttribute
```

## Summary

Internal name of the key to store angles in, allows the helper to be rotated.
## Constructors

```c#
BaseTransformAttribute( string name) 
```
No Summary
## Properties

```c#
string Angles { get; set; } 
```
Internal name of the key to store angles in, allows the helper to be rotated.
```c#
string Attachment { get; set; } 
```
Internal name of the key that dictates which attachment to use as parent for position/angles.
```c#
string Bone { get; set; } 
```
Internal name of the key that dictates which bone to use as parent for position/angles.
```c#
string Origin { get; set; } 
```
Internal name of the key to store position in, if set, allows the helper to be moved.
## Methods

```c#
protected override void AddTransform( StringBuilder sb) 
```
OverridesBaseModelDocAttribute.AddTransformInternal, used to add multi level key-values.
## Inheriting Types

