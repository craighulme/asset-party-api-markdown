# DescriptionAttribute

## ```c#
Implements IDescriptionProvider, IUninheritable
```

## Summary

Sets the description of a type or a type member. This attribute is usually applied automatically by codegen based on the XML comment of the type or member.
This info can then be retrieved via DisplayInfo library.
## Constructors

```c#
DescriptionAttribute( string value) 
```
No Summary
## Properties

```c#
string Value { get; set; } 
```
ImplementsIDescriptionProvider.ValueThe description.
