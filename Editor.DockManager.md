# DockManager

## ```c#
Derives from Widget
```

## Summary

A list of dock types that are registered.
## Constructors

```c#
DockManager( Widget parent = null) 
```
No Summary
## Properties

```c#
IEnumerable<DockInfo> DockTypes { get; } 
```
A list of dock types that are registered.
```c#
string State { get; set; } 
```
A JSON string representing the entire state of the dock manager, i.e. position of all the docks, etc.
## Methods

```c#
void AddDock( Widget sibling, Widget window, DockArea dockArea = 5, DockProperty properties = 0, float split = 0.5) 
```
Add a window next (or on top of) to the specified window.
```c#
void Clear( ) 
```
Clear the known widgets, reset manager to an empty state.
```c#
T Create<T,>( ) 
```
Creates a widget by type
```c#
Widget GetDockWidget( string name) 
```
Get an active, created dock
```c#
bool IsDockOpen( string title) 
```
Whether the given dock-able window is visible or not.
```c#
bool RaiseDock( string name) 
```
Raise this dock to the front of any tabs.
```c#
void RegisterDockType( string name, string icon, Func<Widget> create, bool deleteOnClose = true) 
```
Register a type of dock for the backend to be able to create.
```c#
void SetDockState( string name, bool visible) 
```
Set dock as visible, or hidden, by name.
```c#
void UnregisterDockType( string name) 
```
Unregister a dock type.
## Nested Types

