# VarUnmanaged<T>

## ```c#
Derives from Var
```

## Summary

A fixed size Plain Old Data variable. Can be a built in type or a struct.
## Type Parameters

```c#
T is ValueType, new(), 
```
No Summary
## Constructors

```c#
VarUnmanaged( ) 
```
No Summary
```c#
VarUnmanaged( T defaultValue) 
```
No Summary
## Fields

```c#
T Value
```
No Summary
## Methods

```c#
T& GetValue( ) 
```
No Summary
```c#
void SetValue( in T val) 
```
No Summary
```c#
override string ToString( ) 
```
OverridesVar.ToString
