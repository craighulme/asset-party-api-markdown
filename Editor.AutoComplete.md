# AutoComplete

## 
```c#
Derives from Menu
```

## Summary

The text has changed - fill in the options
## Constructors

```c#
AutoComplete( Widget parent) 
```
No Summary
## Fields

```c#
Action<Menu, string> OnBuildOptions
```
The text has changed - fill in the options
```c#
Action<string> OnOptionSelected
```
You should hook this up to change the text on your control
## Properties

```c#
bool HasAutocompleteOptions { get; protected set; } 
```
No Summary
```c#
int MinimumLength { get; set; } 
```
No Summary
```c#
Vector2 OpenOffset { get; set; } 
```
No Summary
## Methods

```c#
void OnAutoComplete( string newPrefix, Vector2 screenPosition) 
```
No Summary
```c#
void OnGlobalMousePressed( ) 
```
Called when the mouse is pressed. Will hide this window if we clicked on anything
except ourselves or our parent control.
```c#
void OnParentBlur( ) 
```
Call this when the widget that spawns this blurs, so we can hide ourself
```c#
void OnParentKeyPress( KeyEvent e) 
```
You should call this from the parent when a key is pressed. Will forward
the appropriate keys to us and accept the event.
```c#
void OpenAbove( Vector2 position) 
```
Open above this position
```c#
override Option AddOption( string name, string icon = null, Action action = null, string shortcut = null) 
```
OverridesMenu.AddOptionAdd an option for this autocomplete
