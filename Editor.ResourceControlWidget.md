# ResourceControlWidget

## ```c#
Derives from ControlWidget
```

## Summary

OverridesControlWidget.IsControlButton
## Constructors

```c#
ResourceControlWidget( SerializedProperty property) 
```
No Summary
## Properties

```c#
override bool IsControlButton { get; } 
```
OverridesControlWidget.IsControlButton
## Methods

```c#
protected override void OnContextMenu( ContextMenuEvent e) 
```
OverridesControlWidget.OnContextMenuCalled afterWidget.OnMouseRightClick, for the purposes of opening a context menu.
```c#
override void OnDragDrop( DragEvent ev) 
```
OverridesWidget.OnDragDropSomething was dragged and dropped on this widget. Apply the data here, if its valid.RequiresWidget.AcceptDropsto function.
```c#
override void OnDragHover( DragEvent ev) 
```
OverridesWidget.OnDragHoverCursor with drag and drop data moved on this widget.RequiresWidget.AcceptDropsto function.
```c#
protected override void OnDragStart( ) 
```
OverridesWidget.OnDragStartCalled when dragging.Widget.IsDraggableshould be true.
```c#
protected override void OnMouseClick( MouseEvent e) 
```
OverridesWidget.OnMouseClickCalled when this widget is left clicked (on mouse release).
```c#
protected override void PaintControl( ) 
```
OverridesControlWidget.PaintControl
