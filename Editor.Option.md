# Option

## Derives from QObject

## Summary

Called when this option was toggled.
## Constructors

```c#
Option( QObject parent, string title = null, string icon = null, Action action = null) 
```
No Summary
```c#
Option( string title = null, string icon = null, Action action = null) 
```
No Summary
## Fields

```c#
Action<bool> Toggled
```
Called when this option was toggled.
```c#
Action Triggered
```
Called when this option was clicked..
## Properties

```c#
bool Checkable { get; set; } 
```
Whether this option is a toggle option.Option.Checked.
```c#
bool Checked { get; set; } 
```
Whether this option is toggled/checked.Option.Checkable.
```c#
bool Enabled { get; set; } 
```
Whether this option can be clicked. Will also be visually different.
```c#
string Icon { get; set; } 
```
The icon for this option.
```c#
string IconText { get; set; } 
```
Text to display ifOption.Textis empty.
```c#
string Shortcut { get; set; } 
```
"Ctrl+S", "Shift+Ctrl+Z", "Ctrl+Shift+G"
```c#
string StatusText { get; set; } 
```
If set, hovering over this widget will set the text of aEditor.StatusBarof the window the widget belongs to.
```c#
string Text { get; set; } 
```
Text for this option.
```c#
string Tooltip { get; set; } 
```
If set, this text will be displayed after a certain delay of hovering this widget with the mouse cursor.
## Methods

```c#
protected virtual void OnToggled( bool b) 
```
Called when this option was toggled.
```c#
protected virtual void OnTriggered( ) 
```
Called when this option was clicked..
