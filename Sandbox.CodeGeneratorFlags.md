# CodeGeneratorFlags

## Derives from Enum

## Summary

Used to specify what type of code generation to perform.
## Fields

```c#
static CodeGeneratorFlags Instance = 16
```
Apply this to an instance property or method.
```c#
static CodeGeneratorFlags Static = 8
```
Apply this to a static property or method.
```c#
static CodeGeneratorFlags WrapMethod = 4
```
Wrap a method call.
```c#
static CodeGeneratorFlags WrapPropertyGet = 1
```
Wrap the get accessor of a property.
```c#
static CodeGeneratorFlags WrapPropertySet = 2
```
Wrap the set accessor of a property.
## Referencing Members

```c#
CodeGeneratorAttribute.CodeGeneratorAttribute( CodeGeneratorFlags, string ) 
```
```c#
CodeGeneratorFlags = CodeGeneratorAttribute.Type { get; init; } 
```
