# MorphCollection

## ```c#
Derives from object
```

## Summary

Used to access and manipulate morphs.
## Constructors

```c#
protected MorphCollection( ) 
```
No Summary
## Properties

```c#
abstract int Count { get; } 
```
Amount of morphs.
## Methods

```c#
abstract float Get( int i) 
```
Get indexed morph value (Note: Currently, this only gets the override morph value)
```c#
abstract float Get( string name) 
```
Get named morph value (Note: Currently, this only gets the override morph value)
```c#
abstract string GetName( int index) 
```
Retrieve name of a morph at given index.
```c#
abstract void Reset( int i) 
```
Reset morph number i to its default value.
```c#
abstract void Reset( string name) 
```
Reset named morph to its default value.
```c#
abstract void ResetAll( ) 
```
Reset all morphs to their default values.
```c#
abstract void Set( int i, float weight) 
```
Set indexed morph to this value.
```c#
abstract void Set( string name, float weight) 
```
Set named morph to this value.
