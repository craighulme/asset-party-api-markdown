# BaseScrollWidget

## ```c#
Derives from Frame
```

## Summary

The horizontal scroll bar.
## Constructors

```c#
BaseScrollWidget( Widget parent = null) 
```
No Summary
## Properties

```c#
ScrollBar HorizontalScrollbar { get; init; } 
```
The horizontal scroll bar.
```c#
ScrollbarMode HorizontalScrollbarMode { get; set; } 
```
BaseScrollWidget.HorizontalScrollbarmode.
```c#
bool SmoothScrolling { get; set; } 
```
No Summary
```c#
float SmoothScrollTarget { get; set; } 
```
The smooth scrolling wants to move by this amount
```c#
ScrollBar VerticalScrollbar { get; init; } 
```
The vertical scroll bar.
```c#
ScrollbarMode VerticalScrollbarMode { get; set; } 
```
BaseScrollWidget.VerticalScrollbarmode.
## Methods

```c#
protected virtual void OnScrollChanged( ) 
```
Called when the scroll position has changed.
```c#
virtual void ScrollingFrame( ) 
```
No Summary
```c#
protected override void OnKeyPress( KeyEvent e) 
```
OverridesWidget.OnKeyPressA key has been pressed. Your widget needs keyboard focus for this to be called - see FocusMode.
```c#
protected override void OnWheel( WheelEvent e) 
```
OverridesWidget.OnWheelMouse wheel was scrolled while the mouse cursor was over this widget.
```c#
override void Update( ) 
```
OverridesWidget.UpdateTell this widget that shit changed and it needs to redraw
## Inheriting Types

