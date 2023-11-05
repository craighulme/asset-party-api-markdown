# CompilerOutput

## Derives from ValueType
Implements IEquatable< CompilerOutput>

## Summary

OverridesValueType.Equals
## Constructors

```c#
CompilerOutput( string Name, byte[] Assembly, string XmlDocumentation) 
```
No Summary
## Properties

```c#
byte[] Assembly { get; set; } 
```
No Summary
```c#
string Name { get; set; } 
```
No Summary
```c#
string XmlDocumentation { get; set; } 
```
No Summary
## Methods

```c#
void Deconstruct( out string Name, out byte[] Assembly, out string XmlDocumentation) 
```
No Summary
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( CompilerOutput other) 
```
OverridesValueType.Equals
```c#
override int GetHashCode( ) 
```
OverridesValueType.GetHashCode
```c#
override string ToString( ) 
```
OverridesValueType.ToString
## Operators

```c#
bool ==( CompilerOutput left, CompilerOutput right) 
```
No Summary
```c#
bool !=( CompilerOutput left, CompilerOutput right) 
```
No Summary
