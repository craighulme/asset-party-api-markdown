# BoxSizeAttribute

## Derives from MetaDataAttribute

## Summary

For point entities without visualization (model/sprite), sets the size of the box the entity will appear as in Hammer.
## Constructors

```c#
BoxSizeAttribute( float size) 
```
No Summary
```c#
BoxSizeAttribute( float minsX, float minsY, float minsZ) 
```
No Summary
```c#
BoxSizeAttribute( float minsX, float minsY, float minsZ, float maxsX, float maxsY, float maxsZ) 
```
No Summary
## Properties

```c#
string Maxs { get; set; } 
```
No Summary
```c#
string Mins { get; set; } 
```
No Summary
## Methods

```c#
override void AddHelpers( List<Tuple<string, string[]>> helpers) 
```
OverridesMetaDataAttribute.AddHelpers
