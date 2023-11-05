# Menu

## 
```c#
Derives from Widget
```

## Summary

Add a widget as an action to the menu.Some widgets such asEditor.WidgetandEditor.LineEditrequireWidget.OnMouseReleasedto setMouseEvent.Acceptedtotrueto prevent the menu from closing.
## Constructors

```c#
Menu( Widget parent = null) 
```
No Summary
```c#
Menu( string title, Widget parent = null) 
```
No Summary
## Properties

```c#
bool HasMenus { get; } 
```
No Summary
```c#
bool HasOptions { get; } 
```
No Summary
```c#
string Icon { get; set; } 
```
No Summary
```c#
Option SelectedOption { get; } 
```
No Summary
```c#
string Title { get; set; } 
```
No Summary
## Methods

```c#
virtual Option AddOption( string name, string icon = null, Action action = null, string shortcut = null) 
```
No Summary
```c#
virtual Option AddOption( Option option) 
```
No Summary
```c#
protected virtual void OnAboutToHide( ) 
```
No Summary
```c#
protected virtual void OnAboutToShow( ) 
```
No Summary
```c#
Menu AddMenu( string name, string icon = null) 
```
No Summary
```c#
Option AddSeparator( ) 
```
No Summary
```c#
T AddWidget<T,>( T widget) 
```
Add a widget as an action to the menu.Some widgets such asEditor.WidgetandEditor.LineEditrequireWidget.OnMouseReleasedto setMouseEvent.Acceptedtotrueto prevent the menu from closing.
```c#
void Clear( ) 
```
No Summary
```c#
Menu FindOrCreateMenu( string name) 
```
No Summary
```c#
Option GetOption( string name) 
```
No Summary
```c#
void GetPathTo( string path, List<Menu> list) 
```
No Summary
```c#
void OpenAt( Vector2 position, bool modal = true) 
```
No Summary
```c#
void OpenAtCursor( bool modal = false) 
```
Open this menu at the mouse cursor position
```c#
void RemoveMenus( ) 
```
Remove all menus
```c#
void RemoveOption( string name) 
```
No Summary
```c#
void RemoveOption( Option option) 
```
No Summary
```c#
void RemoveOptions( ) 
```
Remove all options
## Events

```c#
AboutToHide( ) 
```
No Summary
```c#
AboutToShow( ) 
```
No Summary
## Inheriting Types

