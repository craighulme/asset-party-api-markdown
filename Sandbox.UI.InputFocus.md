# InputFocus

## 
```c#
Derives from object
```

## Summary

Handles input focus forUI.Panels.
## Properties

```c#
static Panel Current { get; } 
```
The panel that currently has input focus.
```c#
static Panel Next { get; } 
```
The panel that will have the input focus next.
## Methods

```c#
static bool Clear( Panel panel) 
```
Clear focus away from this panel.
```c#
static bool Set( Panel panel) 
```
Set the focus to this panel (or its nearest ancestor with AcceptsFocus).
Note thatInputFocus.Currentwon't change until the next frame.
