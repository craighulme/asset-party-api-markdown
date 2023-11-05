# LineEdit

## 
```c#
Derives from Widget
```

## Summary

A single line text entry. SeeEditor.TextEditfor multi line version.
## Constructors

```c#
LineEdit( Widget parent = null) 
```
No Summary
```c#
LineEdit( string title, Widget parent = null) 
```
No Summary
## Properties

```c#
virtual string Value { get; set; } 
```
Alias ofLineEdit.Text, except disallows setting text whenWidget.IsFocusedistrue.
```c#
TextFlag Alignment { get; set; } 
```
No Summary
```c#
AutoComplete AutoComplete { get; set; } 
```
No Summary
```c#
bool AutoCompleteVisible { get; } 
```
Whether theauto completeEditor.Menuis visible or not.
```c#
bool ClearButtonEnabled { get; set; } 
```
Show a button to clear the text input when it is not empty.
```c#
int CursorPosition { get; set; } 
```
Position of the text cursor, at which newly typed letters will be inserted.
```c#
Rect CursorRect { get; } 
```
No Summary
```c#
string DisplayText { get; } 
```
No Summary
```c#
Widget ForwardNavigationEvents { get; set; } 
```
Forward up, down and enter keys to this control. This is useful if you have a
search box that you want to also allow to navigate a list of items.
```c#
bool HasSelectedText { get; } 
```
Whether the user has any text selected within this text entry.
```c#
string HistoryCookie { get; set; } 
```
No Summary
```c#
bool HistoryVisible { get; } 
```
True if history menu is visible
```c#
int MaxHistoryItems { get; set; } 
```
if set > 1 we will support history items (which you need to add using AddHistory)
```c#
int MaxLength { get; set; } 
```
User entered text can never be longer than this many characters (not bytes).
```c#
string PlaceholderText { get; set; } 
```
The placeholder text, it will be displayed only when the text entry is empty.
Typically used to as a short description of the expected input, or as an example input.
```c#
string RegexValidator { set; } 
```
No Summary
```c#
string SelectedText { get; } 
```
The selected text, if any.
```c#
int SelectionEnd { get; } 
```
Character at which the text selection ends, or -1 if there is no selection.
```c#
int SelectionStart { get; } 
```
Character at which the text selection begins, or -1 if there is no selection.
```c#
string Text { get; set; } 
```
The text of this text entry.
```c#
override bool ReadOnly { get; set; } 
```
OverridesWidget.ReadOnlyMakes the widget read only. I.e. You can copy text of a text entry, but can't edit it.
Applies retroactively to all children.
## Methods

```c#
protected virtual void OnEditingFinished( ) 
```
The text entry lost keyboard focus.
```c#
protected virtual void OnReturnPressed( ) 
```
Called when the user presses the return (Enter) key.
```c#
protected virtual void OnTextChanged( string value) 
```
Called when the input text changes.
```c#
protected virtual void OnTextEdited( string value) 
```
Called when the text was edited.
```c#
virtual void RestoreHistoryFromCookie( ) 
```
No Summary
```c#
virtual void SaveHistoryCookie( ) 
```
No Summary
```c#
void AddHistory( string text) 
```
No Summary
```c#
Option AddOptionToEnd( Option option) 
```
No Summary
```c#
Option AddOptionToFront( Option option) 
```
No Summary
```c#
void Clear( ) 
```
Clear the text.
```c#
void Copy( ) 
```
No Summary
```c#
void Cut( ) 
```
No Summary
```c#
void Deselect( ) 
```
De-select all of the text.
```c#
void Insert( string val) 
```
No Summary
```c#
void Paste( ) 
```
No Summary
```c#
void Redo( ) 
```
No Summary
```c#
void SelectAll( ) 
```
Select all of the text.
```c#
void SetAutoComplete( Action<Menu, string> func) 
```
No Summary
```c#
void SetValidator( string str) 
```
No Summary
```c#
void Undo( ) 
```
No Summary
```c#
protected override bool FocusNext( ) 
```
OverridesWidget.FocusNextIf we have our menus open, let use tab/shift tab to navigate instead of switching to next control
```c#
protected override bool FocusPrevious( ) 
```
OverridesWidget.FocusPreviousIf we have our menus open, let use tab/shift tab to navigate instead of switching to next control
```c#
protected override void OnBlur( FocusChangeReason reason) 
```
OverridesWidget.OnBlurCalled when the widget loses keyboard focus.
```c#
protected override void OnFocus( FocusChangeReason reason) 
```
OverridesWidget.OnFocusCalled when the widget gains keyboard focus.
```c#
protected override void OnKeyPress( KeyEvent e) 
```
OverridesWidget.OnKeyPressA key has been pressed. Your widget needs keyboard focus for this to be called - see FocusMode.
## Events

```c#
EditingFinished( ) 
```
The text entry lost keyboard focus.
```c#
EditingStarted( ) 
```
The text entry received keyboard focus.
```c#
ReturnPressed( ) 
```
Called when the text was edited.
```c#
TextChanged( string obj) 
```
Called when the input text changes.
```c#
TextEdited( string obj) 
```
Called when the text was edited.
## Inheriting Types

