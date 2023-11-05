# IComponent

## Is interface

## Summary

Whether this component is enabled or not.
## Properties

```c#
abstract bool Enabled { get; set; } 
```
Whether this component is enabled or not.
```c#
abstract bool IsClientOnly { get; } 
```
True if this component only exists on the client
```c#
abstract bool IsServerOnly { get; } 
```
True if this component only exists on the server
```c#
abstract string Name { get; set; } 
```
Name of the component, will be shown in entity inspector
