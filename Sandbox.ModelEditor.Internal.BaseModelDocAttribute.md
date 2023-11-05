# BaseModelDocAttribute

## Derives from MetaDataAttribute

## Summary

Add generic key-values to the helper.
## Constructors

```c#
BaseModelDocAttribute( string name) 
```
No Summary
## Methods

```c#
protected virtual void AddKeys( Dictionary<string, object> dict) 
```
Add generic key-values to the helper.
```c#
protected virtual void AddTransform( StringBuilder sb) 
```
Internal, used to add multi level key-values.
```c#
override void AddHelpers( List<Tuple<string, string[]>> helpers) 
```
OverridesMetaDataAttribute.AddHelpers
## Inheriting Types

