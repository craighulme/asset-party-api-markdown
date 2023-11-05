# Link

## 
```c#
Derives from object
```

## Summary

Joins two proxies together, so one can be updated from the other (or both from each other)
## Properties

```c#
bool IsValid { get; } 
```
This is updated in tick. Will return false if either binding is invalid. Bindings become
invalid if the object is garbage collected or is an IValid and made invalid.
```c#
Proxy Left { get; } 
```
The primary binding. Changes to this value always take priority over the other.
```c#
bool OneWay { get; } 
```
True if this should only update from left to right.
```c#
Proxy Right { get; } 
```
The secondary binding, if we're OneWay then this will only ever be written to.
## Methods

```c#
override string ToString( ) 
```
OverridesObject.ToString
