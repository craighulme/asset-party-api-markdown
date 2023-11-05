# OrthoBoundsHelperAttribute

## 
```c#
Derives from MetaDataAttribute
```

## Summary

Creates a resizable box helper that represents an orthographic projection from the entity's origin in Hammer.
The size of the bounding box as defined by the level designer is put into given keys/properties.
## Constructors

```c#
OrthoBoundsHelperAttribute( string rangeKey, string widthKey, string heightKey) 
```
No Summary
## Properties

```c#
string HeightKey { get; set; } 
```
No Summary
```c#
string RangeKey { get; set; } 
```
No Summary
```c#
string WidthKey { get; set; } 
```
No Summary
## Methods

```c#
override void AddHelpers( List<Tuple<string, string[]>> helpers) 
```
OverridesMetaDataAttribute.AddHelpers
