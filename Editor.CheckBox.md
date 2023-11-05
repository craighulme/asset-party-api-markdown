# CheckBox

## Derives from Widget

## Summary

A generic checkbox widget.
## Constructors

```c#
CheckBox( Widget parent = null) 
```
No Summary
```c#
CheckBox( string title, Widget parent = null) 
```
No Summary
```c#
CheckBox( string title, string icon, Widget parent = null) 
```
No Summary
## Fields

```c#
Action Clicked
```
Called when checkbox was clicked, on release.
```c#
Action Pressed
```
Called when checkbox was pressed down.
```c#
Action Released
```
Called when checkbox was released.
```c#
Action<CheckState> StateChanged
```
Called when theCheckBox.Stateof the checkbox states.
```c#
Action Toggled
```
Called when checkbox gets toggled on or off.
## Properties

```c#
string Icon { set; } 
```
Name of a material icon to be drawn in front of the checkbox label.
```c#
CheckState State { get; set; } 
```
Current state of this checkbox.
```c#
string Text { get; set; } 
```
The checkbox label.
```c#
bool TriState { get; set; } 
```
Enable the third state, the half checked half not checked state.
Disabled by default
```c#
bool Value { get; set; } 
```
Whether the checkbox is checked or not.
## Methods

```c#
protected virtual void OnClicked( ) 
```
Called when checkbox was clicked, on release.
```c#
protected virtual void OnPressed( ) 
```
Called when checkbox was pressed down.
```c#
protected virtual void OnReleased( ) 
```
Called when checkbox was released.
```c#
protected virtual void OnStateChanged( CheckState state) 
```
Called when theCheckBox.Stateof the checkbox states.
```c#
protected virtual void OnToggled( ) 
```
Called when checkbox gets toggled on or off.
## Inheriting Types

