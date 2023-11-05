# CodeGeneratorAttribute

## 
```c#
Derives from Attribute
```

## Summary

An attribute that can be added to a custom System.Attribute class for special code generation behavior.
They'll then be applied to methods and properties when they are decorated with that attribute.
## Constructors

```c#
CodeGeneratorAttribute( CodeGeneratorFlags type, string callbackName) 
```
Perform code generation for a method or property.
## Properties

```c#
string CallbackName { get; init; } 
```
No Summary
```c#
CodeGeneratorFlags Type { get; init; } 
```
No Summary
