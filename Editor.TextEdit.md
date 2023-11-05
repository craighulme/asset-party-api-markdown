# TextEdit

## Derives from Widget

## Summary

A multi-line text entry. SeeEditor.LineEditfor a single line version.
## Constructors

```c#
TextEdit( Widget parent = null) 
```
No Summary
## Properties

```c#
bool BackgroundVisible { get; set; } 
```
No Summary
```c#
bool CenterOnScroll { get; set; } 
```
No Summary
```c#
bool Editable { get; set; } 
```
No Summary
```c#
ScrollBar HorizontalScrollbar { get; init; } 
```
No Summary
```c#
ScrollbarMode HorizontalScrollbarMode { get; set; } 
```
No Summary
```c#
string Html { get; set; } 
```
No Summary
```c#
bool LinksClickable { get; set; } 
```
No Summary
```c#
int MaximumBlockCount { get; set; } 
```
No Summary
```c#
string PlaceholderText { get; set; } 
```
No Summary
```c#
string PlainText { get; set; } 
```
No Summary
```c#
float TabSize { get; set; } 
```
No Summary
```c#
bool TextSelectable { get; set; } 
```
No Summary
```c#
ScrollBar VerticalScrollbar { get; init; } 
```
No Summary
```c#
ScrollbarMode VerticalScrollbarMode { get; set; } 
```
No Summary
```c#
override CursorShape Cursor { get; set; } 
```
OverridesWidget.CursorCursor override for this widget.
```c#
override bool ReadOnly { get; set; } 
```
OverridesWidget.ReadOnlyMakes the widget read only. I.e. You can copy text of a text entry, but can't edit it.
Applies retroactively to all children.
## Methods

```c#
virtual void Clear( ) 
```
No Summary
```c#
void AppendHtml( string html) 
```
No Summary
```c#
void AppendPlainText( string text) 
```
No Summary
```c#
void CenterOnCursor( ) 
```
No Summary
```c#
string GetAnchorAt( Vector2 point) 
```
No Summary
```c#
TextCursor GetCursorAtBlock( int block) 
```
No Summary
```c#
TextCursor GetCursorAtPosition( Vector2 position) 
```
No Summary
```c#
Rect GetCursorRect( TextCursor cursor) 
```
No Summary
```c#
TextCursor GetTextCursor( ) 
```
No Summary
```c#
void ScrollToBottom( ) 
```
No Summary
```c#
void SelectAll( ) 
```
No Summary
```c#
void SetTextCursor( TextCursor cursor) 
```
No Summary
