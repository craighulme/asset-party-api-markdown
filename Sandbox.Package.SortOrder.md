# SortOrder

## ```c#
Implements IEquatable<SortOrder>
```

## Summary

Describes a sort order which can be used with the package/find api
## Constructors

```c#
SortOrder( string Name, string Title, string Icon) 
```
Describes a sort order which can be used with the package/find api
## Properties

```c#
string Icon { get; set; } 
```
No Summary
```c#
string Name { get; set; } 
```
No Summary
```c#
string Title { get; set; } 
```
No Summary
## Methods

```c#
void Deconstruct( out string Name, out string Title, out string Icon) 
```
No Summary
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( SortOrder other) 
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
bool ==( SortOrder left, SortOrder right) 
```
No Summary
```c#
bool !=( SortOrder left, SortOrder right) 
```
No Summary
