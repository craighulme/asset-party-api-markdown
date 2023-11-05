# IBaseInventory

## ```c#
Is interface
```

## Summary

No Summary
## Properties

```c#
abstract Entity Active { get; } 
```
No Summary
## Methods

```c#
abstract bool Add( Entity ent, bool makeactive = false) 
```
No Summary
```c#
abstract bool Contains( Entity ent) 
```
No Summary
```c#
abstract int Count( ) 
```
No Summary
```c#
abstract void DeleteContents( ) 
```
No Summary
```c#
abstract bool Drop( Entity ent) 
```
No Summary
```c#
abstract Entity DropActive( ) 
```
No Summary
```c#
abstract int GetActiveSlot( ) 
```
No Summary
```c#
abstract Entity GetSlot( int i) 
```
No Summary
```c#
abstract void OnChildAdded( Entity child) 
```
No Summary
```c#
abstract void OnChildRemoved( Entity child) 
```
No Summary
```c#
abstract bool SetActive( Entity ent) 
```
No Summary
```c#
abstract bool SetActiveSlot( int i, bool allowempty) 
```
No Summary
```c#
abstract bool SwitchActiveSlot( int idelta, bool loop) 
```
No Summary
