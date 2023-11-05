# BindSystem

## 
```c#
Derives from object
```

## Summary

Data bind system, bind properties to each other.
## Properties

```c#
Builder Build { get; } 
```
A helper to create binds between two properties (or whatever you want)
```c#
bool CatchExceptions { get; } 
```
If true we'll catch and remove exceptions when testing links instead of
propagating them to the Tick call.
```c#
int LinkCount { get; } 
```
The current amount of active links
```c#
string Name { get; init; } 
```
The debug name given to this system (ie Tools, Client, Server)
```c#
bool ThrottleUpdates { get; } 
```
If true we'll throttle time between link change checks. This should
always be enabled in game, for performance reasons.
## Methods

```c#
Attribute[] FindAttributes<T,>( T obj, string property) 
```
For this object, with this property, find the property
that supplies it and return any attributes set on it.
This is useful for editors to allow them to supply the correct
editor, without having access to the property.
```c#
void Flush( ) 
```
Call a tick with no timer limits, forcing all pending actions to be actioned
```c#
void Tick( ) 
```
Should be called every frame. Will run through the links and check
for changes, then action those changes. Will also remove dead links.
