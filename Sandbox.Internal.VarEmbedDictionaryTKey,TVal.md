# VarEmbedDictionary<TKey,TVal>

## ```c#
Derives from VarContainer
```

## Summary

OverridesVarContainer.CreateVariableFromSlotCreate the right type of variable
## Type Parameters

```c#
TKey
```
No Summary
```c#
TVal is INetworkTable, class, 
```
No Summary
## Constructors

```c#
VarEmbedDictionary( Dictionary<TKey, TVal> defaultValue = null) 
```
No Summary
## Fields

```c#
Dictionary<TVal, VarClass<TVal>> ServerValues
```
No Summary
```c#
ObservableDictionary<TKey, TVal> Value
```
No Summary
## Methods

```c#
IDictionary<TKey, TVal> GetValue( ) 
```
No Summary
```c#
void SetValue( IDictionary<TKey, TVal> val) 
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
override string ToString( ) 
```
OverridesVar.ToString
