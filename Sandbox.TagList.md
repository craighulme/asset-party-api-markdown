# TagList

## Derives from HashSet<string>

## Summary

A wrapped HashSet[string]. A list of strings. Used for custom Entity properties.
## Constructors

```c#
TagList( ) 
```
No Summary
```c#
TagList( string tagStr) 
```
No Summary
## Methods

```c#
void Set( string tag, bool on) 
```
Removes or adds a tag based on the second argument.
```c#
void Toggle( string tag) 
```
Removes a tag if it exists, adds it otherwise.
## Operators

```c#
implicit TagList =( string value) 
```
No Summary
