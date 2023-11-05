# AssetProperty

## 
```c#
Implements IEditorAttribute<ResourceTypeAttribute>
```

## Summary

ImplementsIEditorAttribute<T>.SetEditorAttribute
## Constructors

```c#
AssetProperty( Widget parent) 
```
No Summary
## Fields

```c#
AssetType AssetType
```
No Summary
```c#
string ResourceType
```
No Summary
## Properties

```c#
Asset Asset { get; set; } 
```
No Summary
```c#
string Value { get; set; } 
```
No Summary
## Methods

```c#
virtual void SetEditorAttribute( ResourceTypeAttribute attribute) 
```
ImplementsIEditorAttribute<T>.SetEditorAttribute
```c#
protected override void DoLayout( ) 
```
OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
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
protected override void OnDragStart( ) 
```
OverridesWidget.OnDragStartCalled when dragging.Widget.IsDraggableshould be true.
```c#
protected override void OnMouseClick( MouseEvent e) 
```
OverridesWidget.OnMouseClickCalled when this widget is left clicked (on mouse release).
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
