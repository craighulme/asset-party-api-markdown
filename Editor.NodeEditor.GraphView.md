# GraphView

## ```c#
Derives from GraphicsView
```

## Summary

OverridesWidget.OnContextMenuCalled afterWidget.OnMouseRightClick, for the purposes of opening a context menu.
## Constructors

```c#
GraphView( Widget parent) 
```
No Summary
## Properties

```c#
IGraph Graph { get; set; } 
```
No Summary
## Methods

```c#
protected virtual void OnNodeCreated( BaseNode node) 
```
No Summary
```c#
virtual void PushRedo( ) 
```
No Summary
```c#
virtual void PushUndo( string name) 
```
No Summary
```c#
void AddNodeType<T,>( ) 
```
No Summary
```c#
void AddNodeType( Type type) 
```
No Summary
```c#
void BuildFromNodes( IEnumerable<BaseNode> nodes, Vector2 offset = null, bool select = false) 
```
No Summary
```c#
void CopySelection( ) 
```
No Summary
```c#
CommentUI CreateNewComment( string text, CommentColor color, Vector2 position, Vector2 size) 
```
No Summary
```c#
NodeUI CreateNewNode( Type type, Vector2 position) 
```
No Summary
```c#
protected void CreateNewNode( Type type, Vector2 position, PlugOut nodeOutput, bool selected = true) 
```
No Summary
```c#
void CreateNewReroute( Vector2 position) 
```
No Summary
```c#
void CutSelection( ) 
```
No Summary
```c#
void DeleteNode( NodeUI node) 
```
No Summary
```c#
void DeleteSelection( ) 
```
No Summary
```c#
NodeUI FindNode( BaseNode node) 
```
No Summary
```c#
PlugIn FindPlugIn( string name) 
```
No Summary
```c#
PlugOut FindPlugOut( string name) 
```
No Summary
```c#
HandleConfig GetHandleConfig( Type t) 
```
No Summary
```c#
void PasteSelection( ) 
```
No Summary
```c#
void RebuildFromGraph( ) 
```
No Summary
```c#
void SelectAll( ) 
```
No Summary
```c#
NodeUI SelectNode( BaseNode node) 
```
No Summary
```c#
void SetHandleConfig( Type t, HandleConfig config) 
```
No Summary
```c#
void UpdateNode( BaseNode node) 
```
No Summary
```c#
protected override void OnContextMenu( ContextMenuEvent e) 
```
OverridesWidget.OnContextMenuCalled afterWidget.OnMouseRightClick, for the purposes of opening a context menu.
```c#
override void OnDragDrop( DragEvent ev) 
```
OverridesWidget.OnDragDropSomething was dragged and dropped on this widget. Apply the data here, if its valid.RequiresWidget.AcceptDropsto function.
```c#
override void OnDragHover( DragEvent ev) 
```
OverridesWidget.OnDragHoverCursor with drag and drop data moved on this widget.RequiresWidget.AcceptDropsto function.
```c#
override void OnDragLeave( ) 
```
OverridesWidget.OnDragLeaveCursor with drag and drop data left the bounds of this widget.RequiresWidget.AcceptDropsto function.
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
protected override void OnWheel( WheelEvent e) 
```
OverridesWidget.OnWheelMouse wheel was scrolled while the mouse cursor was over this widget.
## Nested Types

