# GameDataAttribute

## 
```c#
Derives from LibraryAttribute
```

## Summary

Indicates that this class/struct should be available as GenericGameData node in ModelDoc
## Constructors

```c#
GameDataAttribute( string name) 
```
No Summary
## Properties

```c#
bool AllowMultiple { get; set; } 
```
Indicates that this type compiles as list, rather than a single entry in the model.
This will also affect how you retrieve this data via Model.GetData().
