# ClassFileLocationAttribute

## Derives from Attribute

## Summary

Automatically added to codegenerated classes to let them determine their location
This helps when looking for resources relative to them, like style sheets.
Replaced in Sept 2023 by SourceLocationAttribute, which is added to classes and members.
## Constructors

```c#
ClassFileLocationAttribute( string value) 
```
No Summary
## Properties

```c#
string Path { get; set; } 
```
No Summary
## Inheriting Types

