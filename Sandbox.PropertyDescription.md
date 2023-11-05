# PropertyDescription

## 
```c#
Derives from MemberDescription
```

## Summary

Describes a property. We use this class to wrap and return PropertyInfo's that are safe to interact with.Returned byInternal.TypeLibraryandSandbox.TypeDescription.
## Properties

```c#
bool CanRead { get; } 
```
Whether this property can be read.
```c#
bool CanWrite { get; } 
```
Whether this property can be written to.
```c#
Type PropertyType { get; } 
```
Property type.
```c#
override bool IsProperty { get; } 
```
OverridesMemberDescription.IsPropertyTrue if we're a property
## Methods

```c#
bool CheckValidationAttributes( object obj, out string[] errors, string name = null) 
```
Check all System.ComponentModel.DataAnnotations.ValidationAttributes on this property, and get the error messages if there are any.
```c#
object GetValue( object obj) 
```
Get the value of this property on given object.
```c#
void SetValue( object obj, object value) 
```
Set the value of this property on given object.
