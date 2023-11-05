# TagAttribute

## Derives from Attribute

## Summary

Adds a single or multiple tags for this type or member. Tags can then be retrieved via DisplayInfo library.
## Constructors

```c#
TagAttribute( string[] tag) 
```
No Summary
```c#
TagAttribute( string tag) 
```
No Summary
## Properties

```c#
string[] Value { get; } 
```
The tags to add for this type or member.
## Methods

```c#
IEnumerable<string> EnumerateValues( ) 
```
Returns all the tags as an enumerable.
## Inheriting Types

