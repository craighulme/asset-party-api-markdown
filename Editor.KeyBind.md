# KeyBind

## 
```c#
Derives from Widget
```

## Summary

OverridesWidget.OnKeyPressA key has been pressed. Your widget needs keyboard focus for this to be called - see FocusMode.
## Constructors

```c#
KeyBind( string key = null, Widget parent = null) 
```
No Summary
```c#
KeyBind( Widget parent) 
```
No Summary
## Properties

```c#
string Value { get; set; } 
```
No Summary
## Methods

```c#
protected void SetValue( string value) 
```
No Summary
```c#
protected override void OnKeyPress( KeyEvent e) 
```
OverridesWidget.OnKeyPressA key has been pressed. Your widget needs keyboard focus for this to be called - see FocusMode.
```c#
protected override void OnMouseClick( MouseEvent e) 
```
OverridesWidget.OnMouseClickCalled when this widget is left clicked (on mouse release).
```c#
protected override void OnMouseReleased( MouseEvent e) 
```
OverridesWidget.OnMouseReleasedCalled when mouse is released over this widget.
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
```c#
protected override Vector2 SizeHint( ) 
```
OverridesWidget.SizeHintShould return the size this widget really wants to be if it can its way. The default
is that you don't care - and just to return whatever the base value is.
