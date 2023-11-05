# PropertyAttribute

## 
```c#
Implements IClassNameProvider, ITitleProvider, IDescriptionProvider
```

## Summary

The help text for this property.
## Constructors

```c#
PropertyAttribute( ) 
```
No Summary
```c#
PropertyAttribute( string internal_name, string help = null) 
```
No Summary
```c#
PropertyAttribute( string internal_name, string title, string help = null) 
```
No Summary
## Properties

```c#
string Help { get; protected set; } 
```
The help text for this property.
```c#
string Name { get; set; } 
```
The internal name of this property. This should be lowercase with no spaces. If unset the lowercased C# variable name is used.
```c#
string Title { get; set; } 
```
The user friendly name of this property. If unset, it will be auto generated from C# variable name.
