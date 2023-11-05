# ITypeAttribute

## Is interface

## Summary

When applied to an attribute, which is then applied to a type..
This will makeITypeAttribute.TargetTypeset on the attribute upon load.This provides a convenient way to know which type the attribute was attached to.
## Properties

```c#
abstract Type TargetType { get; set; } 
```
The type this attribute was attached to.
## Methods

```c#
virtual void TypeRegister( ) 
```
Called when a class with this attribute is registered via the TypeLibrary.
```c#
virtual void TypeUnregister( ) 
```
Called when a class with this attribute is unregistered via the TypeLibrary.
