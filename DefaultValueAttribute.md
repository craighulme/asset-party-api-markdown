# DefaultValueAttribute

## Derives from Attribute

## Summary

Sometimes with CodeGen we want reflection to be able to get the original initial value
of a property (which is set with {get;set;} = initialvalue;). For this reason sometimes
we'll drop this attribute on that property.
You might want to use this manually for instances where codegen can't define the default
value. This will usually happen for structs like vector and color.. if the default value isn't
defined as a number or string.
## Constructors

```c#
DefaultValueAttribute( object value) 
```
No Summary
## Properties

```c#
object Value { get; } 
```
The default value.
