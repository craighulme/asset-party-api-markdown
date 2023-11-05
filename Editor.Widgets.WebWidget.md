# WebWidget

## 
```c#
Derives from Widget
```

## Summary

A widget that shows a web page.
## Constructors

```c#
WebWidget( Widget parent) 
```
No Summary
## Properties

```c#
WebSurface Surface { get; } 
```
Access to the HTML surface to change URL, etc.
## Methods

```c#
protected override void OnBlur( FocusChangeReason reason) 
```
OverridesWidget.OnBlurCalled when the widget loses keyboard focus.
```c#
override void OnDestroyed( ) 
```
OverridesQObject.OnDestroyed
```c#
protected override void OnFocus( FocusChangeReason reason) 
```
OverridesWidget.OnFocusCalled when the widget gains keyboard focus.
```c#
protected override void OnKeyPress( KeyEvent e) 
```
OverridesWidget.OnKeyPressA key has been pressed. Your widget needs keyboard focus for this to be called - see FocusMode.
```c#
protected override void OnKeyRelease( KeyEvent e) 
```
OverridesWidget.OnKeyReleaseA key has been released.
```c#
protected override void OnMouseMove( MouseEvent e) 
```
OverridesWidget.OnMouseMoveCalled when the mouse cursor is moved while being over this widget.
```c#
protected override void OnMousePress( MouseEvent e) 
```
OverridesWidget.OnMousePressCalled when mouse is pressed over this widget.
```c#
protected override void OnMouseReleased( MouseEvent e) 
```
OverridesWidget.OnMouseReleasedCalled when mouse is released over this widget.
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
```c#
protected override void OnResize( ) 
```
OverridesWidget.OnResizeCalled when the widgets' size was changed.
```c#
protected override void OnWheel( WheelEvent e) 
```
OverridesWidget.OnWheelMouse wheel was scrolled while the mouse cursor was over this widget.
