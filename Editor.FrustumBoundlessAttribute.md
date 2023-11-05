# FrustumBoundlessAttribute

## ```c#
Derives from MetaDataAttribute
```

## Summary

Draws a frustum that doesn't contribute to bounds calculations.
## Constructors

```c#
FrustumBoundlessAttribute( string fovKV, string zNearKV, string zFarKV) 
```
No Summary
## Properties

```c#
string FovKV { get; set; } 
```
No Summary
```c#
string ZFarKV { get; set; } 
```
No Summary
```c#
string ZNearKV { get; set; } 
```
No Summary
## Methods

```c#
override void AddHelpers( List<Tuple<string, string[]>> helpers) 
```
OverridesMetaDataAttribute.AddHelpers
