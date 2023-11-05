# ExpandGroup

## Derives from Widget

## Summary

OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
## Constructors

```c#
ExpandGroup( Widget parent) 
```
No Summary
## Fields

```c#
protected int headerSize
```
No Summary
## Properties

```c#
string Icon { get; set; } 
```
No Summary
```c#
Action OnCreateWidget { get; set; } 
```
No Summary
```c#
string StateCookieName { get; set; } 
```
No Summary
```c#
string Title { get; set; } 
```
No Summary
## Methods

```c#
protected virtual void OnOpenStateChanged( bool newState) 
```
No Summary
```c#
virtual void SetOpenState( bool state) 
```
No Summary
```c#
void SetHeaderSize( int height) 
```
No Summary
```c#
void SetWidget( Widget w) 
```
No Summary
```c#
protected override void DoLayout( ) 
```
OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
```c#
protected override void OnDoubleClick( MouseEvent e) 
```
OverridesWidget.OnDoubleClickCalled when the widget was double clicked with any mouse button.
```c#
protected override void OnMousePress( MouseEvent e) 
```
OverridesWidget.OnMousePressCalled when mouse is pressed over this widget.
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
