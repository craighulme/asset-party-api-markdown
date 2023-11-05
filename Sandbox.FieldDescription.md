# FieldDescription

## 
```c#
Derives from MemberDescription
```

## Summary

Describes a field. We use this class to wrap and return FieldInfo's that are safe to interact with.Returned byInternal.TypeLibraryandSandbox.TypeDescription.
## Properties

```c#
Type FieldType { get; } 
```
Property type.
```c#
override bool IsField { get; } 
```
OverridesMemberDescription.IsFieldTrue if we're a field
## Methods

```c#
object GetValue( object obj) 
```
Get the value of this property on given object.
```c#
void SetValue( object obj, object value) 
```
Set the value of this property on given object.
