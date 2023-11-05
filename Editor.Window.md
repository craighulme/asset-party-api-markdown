# Window

## Derives from Widget

## Summary

A unique identifier for this window, to store the window state across sessions using theCookielibrary.
## Constructors

```c#
Window( Widget parent = null) 
```
No Summary
## Fields

```c#
static List<Window> All
```
No Summary
## Properties

```c#
virtual MenuBar MenuBar { get; set; } 
```
No Summary
```c#
Widget Canvas { get; set; } 
```
No Summary
```c#
bool CloseButtonVisible { get; set; } 
```
No Summary
```c#
bool IsDialog { get; set; } 
```
No Summary
```c#
Widget MenuWidget { get; set; } 
```
No Summary
```c#
bool StartCentered { get; set; } 
```
No Summary
```c#
string StateCookie { get; set; } 
```
A unique identifier for this window, to store the window state across sessions using theCookielibrary.
```c#
StatusBar StatusBar { get; set; } 
```
No Summary
```c#
string Title { get; set; } 
```
No Summary
## Methods

```c#
virtual void RestoreFromStateCookie( ) 
```
Called whenever the window should restore its state via theEditorCookielibrary,
that was previously saved inWindow.SaveToStateCookie.You should useWindow.StateCookiein the cookie name.
```c#
virtual void SaveToStateCookie( ) 
```
Called whenever the window should save its state via theEditorCookielibrary,
to be later restored inWindow.RestoreFromStateCookie. This is useful to carry data across game sessions.You should useWindow.StateCookiein the cookie name.
```c#
void AddToolBar( ToolBar bar, ToolbarPosition position = 4) 
```
No Summary
```c#
void Clear( ) 
```
TODO this was a test, get rid of it
```c#
void RemoveToolBar( ToolBar bar) 
```
No Summary
```c#
void RestoreState( string state) 
```
No Summary
```c#
string SaveState( int version = 0) 
```
No Summary
```c#
override void Close( ) 
```
OverridesWidget.CloseIf a window - will close
```c#
protected override void OnBlur( FocusChangeReason reason) 
```
OverridesWidget.OnBlurCalled when the widget loses keyboard focus.
```c#
protected override void OnClosed( ) 
```
OverridesWidget.OnClosedCalled when a window is closed.
```c#
override void Show( ) 
```
OverridesWidget.ShowMake this widget visible.
## Inheriting Types

