# Button

## Derives from Widget

## Summary

A simple button widget.
## Constructors

```c#
Button( Widget parent = null) 
```
No Summary
```c#
Button( string title, Widget parent = null) 
```
No Summary
```c#
Button( string title, string icon, Widget parent = null) 
```
No Summary
## Fields

```c#
Action Clicked
```
No Summary
```c#
Action Pressed
```
No Summary
```c#
Action Released
```
No Summary
```c#
Action Toggled
```
No Summary
## Properties

```c#
string ButtonType { set; } 
```
Button type, for styling purposes.
```c#
string Icon { set; } 
```
Sets an icon for the button via a filepath.
```c#
bool IsChecked { get; set; } 
```
Whether this button is checked. SeeButton.IsToggle.
```c#
bool IsToggle { get; set; } 
```
Whether this button can be toggled on or off. SeeButton.IsChecked.
```c#
string Text { get; set; } 
```
Text on the button.
## Methods

```c#
protected virtual void OnClicked( ) 
```
No Summary
```c#
protected virtual void OnPressed( ) 
```
No Summary
```c#
protected virtual void OnReleased( ) 
```
No Summary
```c#
protected virtual void OnToggled( ) 
```
No Summary
```c#
void SetIcon( Pixmap pixmap) 
```
Sets an icon for the button via a raw image.
## Nested Types

## Inheriting Types

