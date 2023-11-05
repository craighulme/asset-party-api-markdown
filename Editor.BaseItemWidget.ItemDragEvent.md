# ItemDragEvent

## 
```c#
Derives from ValueType
```

## Summary

If true, this is a drop - not just a hover
## Fields

```c#
ItemEdge DropEdge
```
No Summary
```c#
bool IsDrop
```
If true, this is a drop - not just a hover
```c#
VirtualWidget Item
```
No Summary
```c#
Vector2 LocalPosition
```
No Summary
## Properties

```c#
DragData Data { get; } 
```
No Summary
```c#
bool HasAlt { get; } 
```
No Summary
```c#
bool HasCtrl { get; } 
```
No Summary
```c#
bool HasShift { get; } 
```
No Summary
```c#
KeyboardModifiers KeyboardModifiers { get; } 
```
No Summary
## Referencing Members

```c#
ItemDragEvent = BaseItemWidget.CurrentItemDragEvent { get; } 
```
```c#
virtual DropAction = TreeNode.OnDragDrop( ItemDragEvent ) 
```
```c#
protected virtual DropAction = BaseItemWidget.OnItemDrag( ItemDragEvent ) 
```
```c#
protected override DropAction = TreeView.OnItemDrag( ItemDragEvent ) 
```
