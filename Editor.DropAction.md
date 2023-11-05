# DropAction

## 
```c#
Derives from Enum
```

## Summary

Used to tell the user what kind of action will happen during a drag and drop event on mouse release.
In Windows, these actions will also display text near cursor to let the user know what will happen if they release their mouse button.
## Fields

```c#
static DropAction Copy = 1
```
The data will be copied.
```c#
static DropAction Ignore = 0
```
Ignore this drop action.
```c#
static DropAction Link = 4
```
The data will be linked.
```c#
static DropAction Move = 2
```
The data will be moved.
## Referencing Members

```c#
DropAction = DragEvent.Action { get; set; } 
```
```c#
DropAction = Drag.ExecuteBlocking( ) 
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
