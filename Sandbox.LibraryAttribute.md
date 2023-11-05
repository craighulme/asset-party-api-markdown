# LibraryAttribute

## Derives from Attribute
Implements ITitleProvider, IDescriptionProvider, IClassNameProvider, IUninheritable

## Summary

We use this to provide a nice description in the editor
## Constructors

```c#
LibraryAttribute( ) 
```
No Summary
```c#
LibraryAttribute( string name) 
```
No Summary
## Properties

```c#
string Description { get; set; } 
```
We use this to provide a nice description in the editor
```c#
bool Editable { get; set; } 
```
We use this to filter entities to show in the entity list in the editor
```c#
string FullName { get; } 
```
The full class name
```c#
string Group { get; set; } 
```
We use this to organize groups of entities in the editor
```c#
string Name { get; } 
```
This is the name that will be used to create this class.
If you don't set it via the attribute constructor it will be set
to the name of the class it's attached to
```c#
string Title { get; set; } 
```
A nice presentable name to show
## Inheriting Types

