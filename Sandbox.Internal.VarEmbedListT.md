# VarEmbedList<T>

## 
```c#
Derives from VarContainer
```

## Summary

A list of anything readable/writable with NetRead/NetWrite
## Type Parameters

```c#
T is INetworkTable, class, 
```
No Summary
## Constructors

```c#
VarEmbedList( ) 
```
No Summary
```c#
VarEmbedList( List<T> defaultValue = null) 
```
No Summary
## Fields

```c#
Dictionary<T, VarClass<T>> ServerValues
```
No Summary
```c#
ObservableCollection<T> Value
```
No Summary
## Methods

```c#
IList<T> GetValue( ) 
```
No Summary
```c#
void SetValue( IList<T> val) 
```
No Summary
```c#
protected override Var CreateVariableFromSlot( int location) 
```
OverridesVarContainer.CreateVariableFromSlotCreate the right type of variable
```c#
protected override void OnVariableAdded( Var var) 
```
OverridesVarContainer.OnVariableAddedA variable has been added. The slot is right. We can read it here and do stuff with the result.
```c#
protected override void OnVariableRemoved( Var var) 
```
OverridesVarContainer.OnVariableRemovedA variable has been removed. We can get the value here and do stuff with the result.
```c#
override string ToString( ) 
```
OverridesVar.ToString
