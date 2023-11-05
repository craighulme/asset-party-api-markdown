# Group

## Derives from object
Implements IEquatable<Group>

## Summary

Represents a group of compilers
## Constructors

```c#
protected Group( Group original) 
```
No Summary
```c#
Group( ) 
```
No Summary
## Properties

```c#
ICSharpCompiler[] Compilers { get; } 
```
A list of compilers
```c#
bool Finished { get; } 
```
True if the compile has finished
```c#
string Name { get; } 
```
The name of the group (ie Menu or Tools)
## Methods

```c#
override bool Equals( object obj) 
```
OverridesObject.Equals
```c#
override bool Equals( Group other) 
```
OverridesObject.Equals
```c#
override int GetHashCode( ) 
```
OverridesObject.GetHashCode
```c#
override string ToString( ) 
```
OverridesObject.ToString
## Operators

```c#
bool ==( Group left, Group right) 
```
No Summary
```c#
bool !=( Group left, Group right) 
```
No Summary
