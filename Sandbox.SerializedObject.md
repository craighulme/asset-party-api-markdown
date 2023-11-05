# SerializedObject

## 
```c#
Implements IEnumerable<SerializedProperty>
```

## Summary

An object (or data) that can be accessed as an object
## Constructors

```c#
protected SerializedObject( ) 
```
No Summary
## Fields

```c#
protected List<SerializedProperty> PropertyList
```
No Summary
## Properties

```c#
virtual string TypeIcon { get; } 
```
No Summary
```c#
virtual string TypeName { get; } 
```
No Summary
```c#
virtual string TypeTitle { get; } 
```
No Summary
```c#
PropertyChangedDelegate OnPropertyChanged { get; set; } 
```
No Summary
```c#
SerializedProperty ParentProperty { get; set; } 
```
No Summary
## Methods

```c#
virtual IEnumerator<SerializedProperty> GetEnumerator( ) 
```
ImplementsIEnumerable`1.GetEnumerator
```c#
virtual SerializedProperty GetProperty( string v) 
```
No Summary
```c#
virtual void NoteChanged( SerializedProperty childProperty) 
```
It's good manners for a changed SerializedProperty to tell its parent
on set. That way the parent can cascade changes up the tree. This is
particularly important if the tree includes struct types - because those
values will need to be re-set on any ParentProperty's.
```c#
virtual bool TryGetProperty( string v, out SerializedProperty prop) 
```
No Summary
## Nested Types

## Inheriting Types

