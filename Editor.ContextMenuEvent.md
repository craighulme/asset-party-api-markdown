# ContextMenuEvent

## ```c#
Derives from ValueType
```

## Summary

Information about aEditor.Widgets context menu event.
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
Vector2 ScreenPosition { get; } 
```
Absolute position of the mouse cursor on the screen.
## Referencing Members

```c#
protected virtual void Widget.OnContextMenu( ContextMenuEvent ) 
```
```c#
protected override void AssetProperty.OnContextMenu( ContextMenuEvent ) 
```
```c#
protected override void ControlWidget.OnContextMenu( ContextMenuEvent ) 
```
```c#
protected override void ResourceControlWidget.OnContextMenu( ContextMenuEvent ) 
```
```c#
protected override void ResourceProperty<T>.OnContextMenu( ContextMenuEvent ) 
```
```c#
protected override void ActiveGameRow.OnContextMenu( ContextMenuEvent ) 
```
```c#
protected override void CloudProjectRow.OnContextMenu( ContextMenuEvent ) 
```
```c#
protected override void ProjectRow.OnContextMenu( ContextMenuEvent ) 
```
```c#
protected override void GraphView.OnContextMenu( ContextMenuEvent ) 
```
```c#
protected override void TimelineView.OnContextMenu( ContextMenuEvent ) 
```
