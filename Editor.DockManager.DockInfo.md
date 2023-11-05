# DockInfo

## ```c#
Derives from object
```

## Summary

Description of a dock that is available to create by the backend.
## Constructors

```c#
DockInfo( ) 
```
No Summary
## Properties

```c#
Func<Widget> CreateAction { get; set; } 
```
Called when the window wants to create this dock but it doesn't exist.
```c#
bool DeleteOnClose { get; set; } 
```
If true we'll delete the widget when it's closed. Otherwise it'll just be hidden.
```c#
string Icon { get; set; } 
```
Icon to show in the menu.
```c#
string Title { get; set; } 
```
This is what the dock will be shown as in the menu - but also what it will be referenced as internally.
