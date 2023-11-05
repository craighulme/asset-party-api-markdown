# DockWindow

## ```c#
Derives from Window
```

## Summary

A window that is built from docking windows
## Constructors

```c#
DockWindow( ) 
```
No Summary
## Properties

```c#
DockManager DockManager { get; init; } 
```
The dock manager for this window, that is automatically created.
## Methods

```c#
protected virtual void RestoreDefaultDockLayout( ) 
```
Override to apply a default layout to your window. This is called automatically from
RestoreFromStateCookie if there is no cookie set.
```c#
void CreateDynamicViewMenu( Menu menu) 
```
Create a viewmenu dynamically, with common options
```c#
override void RestoreFromStateCookie( ) 
```
OverridesWindow.RestoreFromStateCookieCalled whenever the window should restore its state via theEditorCookielibrary,
that was previously saved inWindow.SaveToStateCookie.You should useWindow.StateCookiein the cookie name.
```c#
override void SaveToStateCookie( ) 
```
OverridesWindow.SaveToStateCookieCalled whenever the window should save its state via theEditorCookielibrary,
to be later restored inWindow.RestoreFromStateCookie. This is useful to carry data across game sessions.You should useWindow.StateCookiein the cookie name.
## Inheriting Types

