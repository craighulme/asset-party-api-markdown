# ICSharpCompiler

## 
```c#
Is interface
```

## Summary

Gives access to a c# compiler
## Properties

```c#
abstract bool Building { get; } 
```
Is this addon is still building?
```c#
abstract bool BuildSuccess { get; } 
```
True if building has finished and was successful
```c#
abstract Diagnostic[] Diagnostics { get; } 
```
A list of warnings and errors created by the last build
```c#
abstract string Name { get; } 
```
Name of this assembly. This isn't an assembly name - it should not contain ".dll" etc.
## Nested Types

