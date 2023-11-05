# SerializedProperty

## 
```c#
Derives from object
```

## Summary

Returns true if the current set value differs from the actual value
## Constructors

```c#
SerializedProperty( ) 
```
No Summary
## Properties

```c#
virtual AsAccessor& As { get; } 
```
No Summary
```c#
virtual string Description { get; } 
```
No Summary
```c#
virtual string DisplayName { get; } 
```
No Summary
```c#
virtual string GroupName { get; } 
```
No Summary
```c#
virtual bool HasChanges { get; } 
```
Returns true if the current set value differs from the actual value
```c#
virtual string IsEditable { get; } 
```
No Summary
```c#
virtual string Name { get; } 
```
No Summary
```c#
virtual SerializedObject Parent { get; } 
```
No Summary
```c#
virtual Type PropertyType { get; } 
```
No Summary
```c#
virtual string SourceFile { get; } 
```
The source filename, if available
```c#
virtual int SourceLine { get; } 
```
The line in the source file, if available
## Methods

```c#
abstract T GetValue<T,>( T defaultValue = null) 
```
No Summary
```c#
virtual bool HasAttribute<T,>( ) 
```
Return true if the property has this attribute
```c#
virtual bool HasAttribute( Type t) 
```
Return true if the property has this attribute
```c#
abstract void SetValue<T,>( T value) 
```
No Summary
```c#
virtual bool TryGetAsObject( out SerializedObject obj) 
```
Try to convert this property into a serialized object for further editing and exploration
```c#
virtual bool TryGetAttribute<T,>( out T attribute) 
```
Try to get this attribute from the property. Return false on fail.
## Nested Types

