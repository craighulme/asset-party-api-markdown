# BoundsHelperAttribute

## Derives from MetaDataAttribute

## Summary

Creates a resizable box helper in Hammer which outputs the size of the bounding box defined by the level designer into given keys/properties.
You can have multiple of this attribute.
## Constructors

```c#
BoundsHelperAttribute( string minsKey, string maxsKey, bool autoCenter = false, bool worldAliged = false) 
```
Creates a box helper that outputs the size of the bounding box defined by the level designer as mins and maxs
```c#
BoundsHelperAttribute( string extentsKey, bool worldAliged = false) 
```
Creates a box helper that outputs the size of the bounding box defined by the level designer as extents (maxs - mins).
This assumes the entity is in the center of the box.
## Properties

```c#
bool AutoCenter { get; set; } 
```
Always move the entity to the center of the bounds.
```c#
string ExtentsKey { get; set; } 
```
Key (classname) of the entity to store the bounding box as an "extents".
This replacesBoundsHelperAttribute.MinsKeyandBoundsHelperAttribute.MaxsKeyand assumes the entity is in the middle of the bounds.
The output value will be the total size of the bounds on each axis.
```c#
bool IsWorldAligned { get; set; } 
```
Make the bounds AABB (true), not OBB (false). Basically ignores rotation.
```c#
string MaxsKey { get; set; } 
```
Key (classname) of the entity to store the "Maxs" of the bounding box.
```c#
string MinsKey { get; set; } 
```
Key (classname) of the entity to store the "Mins" of the bounding box.
## Methods

```c#
override void AddHelpers( List<Tuple<string, string[]>> helpers) 
```
OverridesMetaDataAttribute.AddHelpers
