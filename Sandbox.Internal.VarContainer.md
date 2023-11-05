# VarContainer

## Is abstract
Derives from Var

## Summary

A network variable that points to a bunch of other variables
## Constructors

```c#
protected VarContainer( ) 
```
No Summary
## Fields

```c#
protected bool NeedsRebuild
```
No Summary
```c#
protected List<Var> Variables
```
No Summary
## Properties

```c#
protected int VariableCount { get; } 
```
No Summary
## Methods

```c#
protected virtual Var CreateVariableFromSlot( int location) 
```
No Summary
```c#
protected virtual void OnVariableAdded( Var var) 
```
No Summary
```c#
protected virtual void OnVariableRemoved( Var var) 
```
No Summary
```c#
protected void AddVariable( Var var, int? location) 
```
No Summary
```c#
protected void ReadVariables( ref NetRead read) 
```
No Summary
```c#
protected void ReleaseVariables( ) 
```
No Summary
## Inheriting Types

