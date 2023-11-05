# Label

## ```c#
Derives from Panel
```

## Summary

A generic text label. Can be made editable.
## Constructors

```c#
Label( ) 
```
No Summary
## Fields

```c#
protected StringInfo StringInfo
```
Information about theLabel.Texton a per-element scale. It handles multi-character Unicode units (graphemes) correctly.
## Properties

```c#
virtual string Text { get; set; } 
```
Text to display on the label.
```c#
int CaretPosition { get; set; } 
```
Position of the text cursor/caret within the text, at which newly typed characters are inserted.
```c#
bool Multiline { get; set; } 
```
Enables multi-line support for editing purposes.
```c#
bool Selectable { get; set; } 
```
Can be selected
```c#
int SelectionEnd { get; set; } 
```
No Summary
```c#
int SelectionStart { get; set; } 
```
No Summary
```c#
bool ShouldDrawSelection { get; set; } 
```
No Summary
```c#
int TextLength { get; } 
```
Amount of characters in the text of the text entry. Not bytes.
```c#
override bool HasContent { get; } 
```
OverridesPanel.HasContentIf true, callsPanel.DrawContent.
## Methods

```c#
virtual void RemoveText( int start, int count) 
```
Remove given amount of characters from the label at givenstartposition.
```c#
virtual void SetText( string text) 
```
CallsText = value
```c#
protected void CaretSantity( ) 
```
Ensure the text caret and selection are in sane positions, that is, not outside of the text bounds.
```c#
Rect GetCaretRect( int i) 
```
No Summary
```c#
int GetLetterAt( Vector2 pos) 
```
No Summary
```c#
int GetLetterAtScreenPosition( Vector2 pos) 
```
No Summary
```c#
string GetSelectedText( ) 
```
Returns the selected text.
```c#
List<int> GetWordBoundaryIndices( ) 
```
Returns a list of positions in the text of each side of each word within theLabel.Text.This is used for Control + Arrow Key navigation.
```c#
bool HasSelection( ) 
```
No Summary
```c#
void InsertText( string text, int pos, int? endpos = null) 
```
Insert given text at given position.
```c#
bool IsNewline( string str) 
```
Returns true if the input string is a 1 or 2 (\r\n) character newline symbol.
PAINDAY TODO: Make this private?
```c#
void MoveCaratPos( int delta, bool select = false) 
```
No Summary
```c#
void MoveCaretLine( int offset_line, bool select) 
```
Move the text caret to next or previous line.
```c#
void MoveCaretPos( int delta, bool select = false) 
```
Move the text caret by given amount.
```c#
void MoveToLineEnd( bool select = false) 
```
Move the text caret to the end of the current line.
```c#
void MoveToLineStart( bool select = false) 
```
Move the text caret to the start of the current line.
```c#
void MoveToWordBoundaryLeft( bool select) 
```
Move the text caret to the closest word start or end to the left of current position.This simulates holding Control key while pressing left arrow key.
```c#
void MoveToWordBoundaryRight( bool select) 
```
Move the text caret to the closest word start or end to the right of current position.This simulates holding Control key while pressing right arrow key.
```c#
void ReplaceSelection( string str) 
```
Replace the currently selected text with given text.
```c#
void SelectWord( int wordPos) 
```
Select a work at given word position.
```c#
void SetCaretPosition( int pos, bool select = false) 
```
Set the text caret position to the given index.
```c#
void SetSelection( int start, int end) 
```
Sets the text selection.
```c#
override void FinalLayout( Vector2 offset) 
```
OverridesPanel.FinalLayoutTakes aUI.LayoutCascadeand returns an outer rect
```c#
override string GetClipboardValue( bool cut) 
```
OverridesPanel.GetClipboardValueIf we have a value that can be copied to the clipboard, return it here.
```c#
override void LanguageChanged( ) 
```
OverridesPanel.LanguageChangedWhen the language changes, if we're token based we need to update to the new phrase.
```c#
override void OnDeleted( ) 
```
OverridesPanel.OnDeletedCalled when the panel is about to be deleted.
```c#
override void SetContent( string value) 
```
OverridesPanel.SetContentCalled by the templating system when an element has content between its tags.
```c#
override void SetProperty( string name, string value) 
```
OverridesPanel.SetPropertySet a property on the panel, such as special properties (class,id,styleandvalue, etc.) and properties of the panel's C# class.
## Inheriting Types

