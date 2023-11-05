# Handle

## Derives from GraphicsItem

## Summary

Paint extra background stuff
## Constructors

```c#
Handle( EditableCurve parent, in Frame k) 
```
No Summary
## Fields

```c#
EditableCurve EditableCurve
```
No Summary
```c#
Frame Frame
```
No Summary
```c#
Tangent In
```
No Summary
```c#
Tangent Out
```
No Summary
## Methods

```c#
virtual void OpenContextMenu( Vector2 pos) 
```
No Summary
```c#
void DeleteHandle( ) 
```
No Summary
```c#
void OnHandleModeChanged( ) 
```
No Summary
```c#
void PaintExtras( ) 
```
Paint extra background stuff
```c#
void SetHandleMode( HandleMode mode) 
```
No Summary
```c#
void SetValue( float x, float y) 
```
Set the value from range scaled values
```c#
protected override void OnHoverEnter( GraphicsHoverEvent e) 
```
OverridesGraphicsItem.OnHoverEnter
```c#
protected override void OnHoverLeave( GraphicsHoverEvent e) 
```
OverridesGraphicsItem.OnHoverLeave
```c#
protected override void OnKeyPress( KeyEvent e) 
```
OverridesGraphicsItem.OnKeyPressA key has been pressed.
```c#
protected override void OnMousePressed( GraphicsMouseEvent e) 
```
OverridesGraphicsItem.OnMousePressed
```c#
protected override void OnMoved( ) 
```
OverridesGraphicsItem.OnMovedItem has been moved by the user dragging it
```c#
protected override void OnPaint( ) 
```
OverridesGraphicsItem.OnPaint
```c#
protected override void OnPositionChanged( ) 
```
OverridesGraphicsItem.OnPositionChanged
```c#
protected override void OnSelectionChanged( ) 
```
OverridesGraphicsItem.OnSelectionChanged
