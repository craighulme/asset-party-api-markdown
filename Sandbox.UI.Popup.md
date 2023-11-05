# Popup

## ```c#
Derives from Panel
```

## Summary

SetsPopup.PopupSource,Popup.PositionandPopup.PopupSourceOffset.
Applies relevant CSS classes.
## Constructors

```c#
Popup( ) 
```
No Summary
```c#
Popup( Panel sourcePanel, PositionMode position, float offset) 
```
SetsPopup.PopupSource,Popup.PositionandPopup.PopupSourceOffset.
Applies relevant CSS classes.
## Fields

```c#
protected Panel Header
```
Header panel that holdsPopup.TitleLabelandPopup.IconPanel.
```c#
protected IconPanel IconPanel
```
Panel that dispalysPopup.Icon.
```c#
protected Label TitleLabel
```
Label that dispalysPopup.Title.
## Properties

```c#
string Icon { get; set; } 
```
If set, will add an unselectable header with given icon andPopup.Title.
```c#
Panel PopupSource { get; set; } 
```
Which panel triggered this popup. Set byPopup.SetPositioningor the constructor.
```c#
float PopupSourceOffset { get; set; } 
```
Offset away fromPopup.PopupSourcebased onPopup.Position.
```c#
PositionMode Position { get; set; } 
```
Positioning mode for this popup.
```c#
Panel SelectedChild { get; set; } 
```
Currently selected option in the popup. Used internally for keyboard navigation.
```c#
string Title { get; set; } 
```
If set, will add an unselectable header with given text andPopup.Icon.
## Methods

```c#
static void CloseAll( Panel exceptThisOne = null) 
```
Close allUI.Popupinstances except for the given one.
```c#
static void ClosePopupsEvent( object obj) 
```
Event listener forui.closepopups.
PAINDAY TODO: Make internal?
```c#
Panel AddOption( string text, Action action = null) 
```
Add an option to this popup with given text and click action.
```c#
Panel AddOption( string text, string icon, Action action = null) 
```
Add an option to this popup with given text, icon and click action.
```c#
void Failure( ) 
```
Closes all panels, marks this one as a failure and closes it.
```c#
void MoveSelection( int dir) 
```
Move selection in given direction.
```c#
void SetPositioning( Panel sourcePanel, PositionMode position, float offset) 
```
SetsPopup.PopupSource,Popup.PositionandPopup.PopupSourceOffset.
Applies relevant CSS classes.
```c#
void Success( ) 
```
Closes all panels, marks this one as a success and closes it.
```c#
override void OnDeleted( ) 
```
OverridesPanel.OnDeletedCalled when the panel is about to be deleted.
```c#
override void OnLayout( ref Rect layoutRect) 
```
OverridesPanel.OnLayoutThis panel has just been laid out. You can modify its position now and it will affect its children.
This is a useful place to restrict shit to the screen etc.
```c#
override void Tick( ) 
```
OverridesPanel.TickCalled every frame. This is your "Think" function.
## Nested Types

