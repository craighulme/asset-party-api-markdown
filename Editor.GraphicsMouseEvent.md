# GraphicsMouseEvent

## Derives from ValueType

## Summary

Information about aEditor.GraphicsItems mouse click event.
## Properties

```c#
bool Accepted { get; set; } 
```
Whether this event should be propagated to parent widgets (false) or not (true).
```c#
MouseButtons Button { get; } 
```
The mouse button that triggered the event.
```c#
MouseButtons Buttons { get; } 
```
The current mouse button state.
```c#
bool HasAlt { get; } 
```
WhetherAltkey was being held down at the time of the event.
```c#
bool HasCtrl { get; } 
```
WhetherControlkey was being held down at the time of the event.
```c#
bool HasShift { get; } 
```
WhetherShiftkey was being held down at the time of the event.
```c#
KeyboardModifiers KeyboardModifiers { get; set; } 
```
The keyboard modifier keys that were held down at the moment the event triggered.
```c#
bool LeftMouseButton { get; } 
```
Whether the event was triggered by the left mouse button.
```c#
Vector2 LocalPosition { get; } 
```
Position of the mouse cursor relative to the widgets top left corner.
```c#
bool MiddleMouseButton { get; } 
```
Whether the event was triggered by the left mouse button.
```c#
bool RightMouseButton { get; } 
```
Whether the event was triggered by the left mouse button.
```c#
Vector2 ScenePosition { get; } 
```
Position of the mouse cursor within the Editor.GraphicsScene.
```c#
Vector2 ScreenPosition { get; } 
```
Absolute position of the mouse cursor on the screen.
## Referencing Members

```c#
Drag.Drag( GraphicsMouseEvent ) 
```
```c#
protected virtual void GraphicsItem.OnMouseMove( GraphicsMouseEvent ) 
```
```c#
protected override void CommentUI.OnMouseMove( GraphicsMouseEvent ) 
```
```c#
protected override void Connection.OnMouseMove( GraphicsMouseEvent ) 
```
```c#
protected override void FloatEditor.OnMouseMove( GraphicsMouseEvent ) 
```
```c#
protected override void PlugOut.OnMouseMove( GraphicsMouseEvent ) 
```
```c#
protected override void ResizableItem.OnMouseMove( GraphicsMouseEvent ) 
```
```c#
protected override void PhonemeItem.OnMouseMove( GraphicsMouseEvent ) 
```
```c#
protected override void Tangent.OnMouseMove( GraphicsMouseEvent ) 
```
```c#
protected virtual void GraphicsItem.OnMousePressed( GraphicsMouseEvent ) 
```
```c#
protected override void ColorEditor.OnMousePressed( GraphicsMouseEvent ) 
```
```c#
protected override void CommentUI.OnMousePressed( GraphicsMouseEvent ) 
```
```c#
protected override void Connection.OnMousePressed( GraphicsMouseEvent ) 
```
```c#
protected override void FloatEditor.OnMousePressed( GraphicsMouseEvent ) 
```
```c#
protected override void NodeUI.OnMousePressed( GraphicsMouseEvent ) 
```
```c#
protected override void PlugOut.OnMousePressed( GraphicsMouseEvent ) 
```
```c#
protected override void ResizableItem.OnMousePressed( GraphicsMouseEvent ) 
```
```c#
protected override void TimeAxis.OnMousePressed( GraphicsMouseEvent ) 
```
```c#
protected override void PhonemeItem.OnMousePressed( GraphicsMouseEvent ) 
```
```c#
protected override void EditableCurve.OnMousePressed( GraphicsMouseEvent ) 
```
```c#
protected override void Comment.OnMousePressed( GraphicsMouseEvent ) 
```
```c#
protected override void Handle.OnMousePressed( GraphicsMouseEvent ) 
```
```c#
protected override void Tangent.OnMousePressed( GraphicsMouseEvent ) 
```
```c#
protected virtual void GraphicsItem.OnMouseReleased( GraphicsMouseEvent ) 
```
```c#
protected override void CommentUI.OnMouseReleased( GraphicsMouseEvent ) 
```
```c#
protected override void Connection.OnMouseReleased( GraphicsMouseEvent ) 
```
```c#
protected override void FloatEditor.OnMouseReleased( GraphicsMouseEvent ) 
```
```c#
protected override void NodeUI.OnMouseReleased( GraphicsMouseEvent ) 
```
```c#
protected override void PlugOut.OnMouseReleased( GraphicsMouseEvent ) 
```
```c#
protected override void ResizableItem.OnMouseReleased( GraphicsMouseEvent ) 
```
```c#
protected override void PhonemeItem.OnMouseReleased( GraphicsMouseEvent ) 
```
```c#
protected override void Tangent.OnMouseReleased( GraphicsMouseEvent ) 
```
