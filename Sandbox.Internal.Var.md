# Var

## ```c#
Derives from object
```

## Summary

This variable has pending changes, waiting to be written to network. This
variable stops dirty variables being added to the write list twice.
## Constructors

```c#
protected Var( ) 
```
No Summary
## Fields

```c#
string Name
```
No Summary
## Properties

```c#
Action<object, object> Callback { get; } 
```
No Summary
```c#
int Index { get; set; } 
```
No Summary
```c#
bool IsDirty { get; protected set; } 
```
This variable has pending changes, waiting to be written to network. This
variable stops dirty variables being added to the write list twice.
```c#
bool IsLocal { get; } 
```
No Summary
```c#
bool IsPredicted { get; } 
```
No Summary
## Methods

```c#
protected virtual void AddToWriteList( ) 
```
Add this variable to the write list
```c#
protected virtual void CheckValueChanged( object oldValue, object newValue) 
```
No Summary
```c#
virtual void SetDirty( bool force = false) 
```
Mark this variable as dirty. Its contents have changed and it needs writing
```c#
protected bool CanChangeValue( ) 
```
No Summary
```c#
protected void OnChanged( object oldValue, object newValue) 
```
No Summary
```c#
void SetCallback<T,>( Action<T, T> callback) 
```
No Summary
```c#
void SetCallback<T,>( Action<T> callback) 
```
No Summary
```c#
void SetCallback<T,>( Action callback) 
```
No Summary
```c#
override string ToString( ) 
```
OverridesObject.ToString
## Inheriting Types

