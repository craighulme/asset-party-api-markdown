# Event

## Is static
Derives from object

## Summary

The event system.
## Methods

```c#
static void Register( object obj) 
```
Register an object to start receiving events
```c#
static void Run( string name) 
```
Run an event.
```c#
static void Run<T,>( string name, T arg0) 
```
Run an event with an argument of arbitrary type.
```c#
static void Run<T,U,>( string name, T arg0, U arg1) 
```
Run an event with 2 arguments of arbitrary type.
```c#
static void Run<T,U,V,>( string name, T arg0, U arg1, V arg2) 
```
Run an event with 3 arguments of arbitrary type.
```c#
static void Unregister( object obj) 
```
Unregister an object, stop reviving events
## Nested Types

