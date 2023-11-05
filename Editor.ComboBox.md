# ComboBox

## 
```c#
Derives from Widget
```

## Summary

OverridesWidget.OnBlurCalled when the widget loses keyboard focus.
## Constructors

```c#
ComboBox( Widget parent = null) 
```
No Summary
## Properties

```c#
bool AllowDuplicates { get; set; } 
```
No Summary
```c#
AutoComplete AutoComplete { get; set; } 
```
No Summary
```c#
int Count { get; } 
```
No Summary
```c#
int CurrentIndex { get; set; } 
```
No Summary
```c#
string CurrentText { get; set; } 
```
No Summary
```c#
bool Editable { get; set; } 
```
No Summary
```c#
InsertMode Insertion { get; set; } 
```
No Summary
```c#
LineEdit LineEdit { get; init; } 
```
No Summary
```c#
int MaxVisibleItems { get; set; } 
```
No Summary
```c#
Action OnReturn { get; } 
```
No Summary
```c#
string StateCookie { get; set; } 
```
No Summary
## Methods

```c#
protected virtual void OnItemChanged( ) 
```
No Summary
```c#
protected virtual void OnTextChanged( ) 
```
No Summary
```c#
virtual void RestoreFromStateCookie( ) 
```
No Summary
```c#
virtual void SaveToStateCookie( ) 
```
No Summary
```c#
void AddItem( string text, string icon = null, Action onSelected = null, string description = null, bool selected = false) 
```
No Summary
```c#
void Clear( ) 
```
No Summary
```c#
void ClearText( ) 
```
No Summary
```c#
int? FindIndex( string text) 
```
No Summary
```c#
void InvokeSelected( ) 
```
No Summary
```c#
void SetAutoComplete( Action<Menu, string> func) 
```
No Summary
```c#
bool TrySelectNamed( string name) 
```
No Summary
```c#
protected override void OnBlur( FocusChangeReason reason) 
```
OverridesWidget.OnBlurCalled when the widget loses keyboard focus.
```c#
protected override void OnKeyPress( KeyEvent e) 
```
OverridesWidget.OnKeyPressA key has been pressed. Your widget needs keyboard focus for this to be called - see FocusMode.
## Events

```c#
ItemChanged( ) 
```
No Summary
```c#
TextChanged( ) 
```
No Summary
## Nested Types

## Inheriting Types

