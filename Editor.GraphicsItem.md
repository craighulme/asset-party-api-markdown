# GraphicsItem

## Is abstract
Derives from object
Implements IValid

## Summary

0,0 means top left, 1,1 means bottom right
## Constructors

```c#
GraphicsItem( GraphicsItem parent = null) 
```
No Summary
## Properties

```c#
virtual Vector2 HandlePosition { get; set; } 
```
0,0 means top left, 1,1 means bottom right
```c#
virtual Vector2 Size { get; set; } 
```
No Summary
```c#
Vector2 Center { get; } 
```
No Summary
```c#
bool Clip { get; set; } 
```
No Summary
```c#
bool ClipChildren { get; set; } 
```
No Summary
```c#
CursorShape Cursor { get; set; } 
```
No Summary
```c#
bool Focusable { get; set; } 
```
Gets keyboard input
```c#
GraphicsView GraphicsView { get; } 
```
No Summary
```c#
bool Hovered { get; } 
```
No Summary
```c#
bool HoverEvents { get; set; } 
```
No Summary
```c#
bool IsValid { get; } 
```
ImplementsIValid.IsValid
```c#
Rect LocalRect { get; } 
```
No Summary
```c#
bool Movable { get; set; } 
```
No Summary
```c#
GraphicsItem Parent { get; set; } 
```
No Summary
```c#
Vector2 Position { get; set; } 
```
No Summary
```c#
float Rotation { get; set; } 
```
No Summary
```c#
float Scale { get; set; } 
```
No Summary
```c#
Rect SceneRect { get; set; } 
```
No Summary
```c#
bool Selectable { get; set; } 
```
No Summary
```c#
bool Selected { get; set; } 
```
No Summary
```c#
string Tooltip { get; set; } 
```
No Summary
```c#
Vector2 ViewPosition { get; } 
```
No Summary
```c#
float ZIndex { get; set; } 
```
No Summary
## Methods

```c#
virtual bool Contains( Vector2 localPos) 
```
No Summary
```c#
protected virtual void OnHoverEnter( GraphicsHoverEvent e) 
```
No Summary
```c#
protected virtual void OnHoverLeave( GraphicsHoverEvent e) 
```
No Summary
```c#
protected virtual void OnHoverMove( GraphicsHoverEvent e) 
```
No Summary
```c#
protected virtual void OnKeyPress( KeyEvent e) 
```
A key has been pressed.
```c#
protected virtual void OnKeyRelease( KeyEvent e) 
```
A key has been released.
```c#
protected virtual void OnMouseMove( GraphicsMouseEvent e) 
```
No Summary
```c#
protected virtual void OnMousePressed( GraphicsMouseEvent e) 
```
No Summary
```c#
protected virtual void OnMouseReleased( GraphicsMouseEvent e) 
```
No Summary
```c#
protected virtual void OnMoved( ) 
```
Item has been moved by the user dragging it
```c#
protected virtual void OnPaint( ) 
```
No Summary
```c#
protected virtual void OnPositionChanged( ) 
```
No Summary
```c#
protected virtual void OnSelectionChanged( ) 
```
No Summary
```c#
protected void AddChild( GraphicsItem i) 
```
No Summary
```c#
Builder Bind( string targetName) 
```
No Summary
```c#
void Destroy( ) 
```
No Summary
```c#
Vector2 FromItem( GraphicsItem item, Vector2 pos) 
```
No Summary
```c#
Vector2 FromParent( Vector2 pos) 
```
No Summary
```c#
Vector2 FromScene( Vector2 pos) 
```
No Summary
```c#
void PrepareGeometryChange( ) 
```
Usually called before resizing items so they paint properly.
```c#
protected void RemoveChild( GraphicsItem i) 
```
No Summary
```c#
Vector2 ToItem( GraphicsItem item, Vector2 pos) 
```
No Summary
```c#
Vector2 ToParent( Vector2 pos) 
```
No Summary
```c#
Vector2 ToScene( Vector2 pos) 
```
No Summary
```c#
void Update( ) 
```
No Summary
## Inheriting Types

