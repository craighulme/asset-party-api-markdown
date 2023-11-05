# GraphicsHoverEvent

## Derives from ValueType

## Summary

Information about aEditor.GraphicsItems mouse hover event.
## Properties

```c#
bool Accepted { get; set; } 
```
Whether this event should be propagated to parent widgets (false) or not (true).
```c#
Vector2 LocalPosition { get; } 
```
Position of the mouse cursor relative to the widgets top left corner.
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
protected virtual void GraphicsItem.OnHoverEnter( GraphicsHoverEvent ) 
```
```c#
protected override void CommentUI.OnHoverEnter( GraphicsHoverEvent ) 
```
```c#
protected override void FloatEditor.OnHoverEnter( GraphicsHoverEvent ) 
```
```c#
protected override void ResizableItem.OnHoverEnter( GraphicsHoverEvent ) 
```
```c#
protected override void PhonemeItem.OnHoverEnter( GraphicsHoverEvent ) 
```
```c#
protected override void Handle.OnHoverEnter( GraphicsHoverEvent ) 
```
```c#
protected virtual void GraphicsItem.OnHoverLeave( GraphicsHoverEvent ) 
```
```c#
protected override void CommentUI.OnHoverLeave( GraphicsHoverEvent ) 
```
```c#
protected override void ResizableItem.OnHoverLeave( GraphicsHoverEvent ) 
```
```c#
protected override void PhonemeItem.OnHoverLeave( GraphicsHoverEvent ) 
```
```c#
protected override void Handle.OnHoverLeave( GraphicsHoverEvent ) 
```
```c#
protected virtual void GraphicsItem.OnHoverMove( GraphicsHoverEvent ) 
```
```c#
protected override void CommentUI.OnHoverMove( GraphicsHoverEvent ) 
```
```c#
protected override void ResizableItem.OnHoverMove( GraphicsHoverEvent ) 
```
```c#
protected override void PhonemeItem.OnHoverMove( GraphicsHoverEvent ) 
```
