# CanEditAttribute

## Derives from Attribute
Implements ITypeAttribute, IUninheritable

## Summary

ImplementsITypeAttribute.TargetTypeThe type this attribute was attached to.
## Constructors

```c#
CanEditAttribute( Type type, string typeName = null) 
```
No Summary
```c#
CanEditAttribute( string typeName) 
```
No Summary
## Properties

```c#
virtual Type TargetType { get; set; } 
```
ImplementsITypeAttribute.TargetTypeThe type this attribute was attached to.
```c#
Type Type { get; init; } 
```
No Summary
```c#
string TypeName { get; init; } 
```
No Summary
## Methods

```c#
static Widget CreateEditorFor( PropertyInfo property, ref object target) 
```
No Summary
```c#
static Widget CreateEditorFor( Type t, IEnumerable<Attribute> attributes = null, Type[] generics = null) 
```
No Summary
```c#
static Widget CreateEditorFor( string name) 
```
No Summary
```c#
static Widget CreateEditorForObject( object obj) 
```
No Summary
