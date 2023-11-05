# ClassNameAttribute

## ```c#
Implements IClassNameProvider, IUninheritable
```

## Summary

Set the class name for this type or member.
This info can then be retrieved via DisplayInfo library.
## Constructors

```c#
ClassNameAttribute( string value) 
```
No Summary
## Properties

```c#
string Value { get; set; } 
```
ImplementsIClassNameProvider.ValueThe class name.
Typically a class name is all lower case, has spaces replaced by underscores (_) or dashes (-) and contains no other special symbols.
