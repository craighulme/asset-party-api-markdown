# TreeView

## 
```c#
Derives from BaseItemWidget
```

## Summary

If true, when an object is selected via SelectItem or dynamically via SelectionOverride, the treeview will
open all the items leading to that item and scroll to it.
## Constructors

```c#
TreeView( Widget parent = null) 
```
No Summary
## Properties

```c#
bool ExpandForSelection { get; set; } 
```
If true, when an object is selected via SelectItem or dynamically via SelectionOverride, the treeview will
open all the items leading to that item and scroll to it.
```c#
float ExpandWidth { get; set; } 
```
Width of the expand/collapse button.
```c#
float IndentWidth { get; set; } 
```
Additional horizontal indent for each subtree level.
```c#
float ItemSpacing { get; set; } 
```
Vertical spacing between each item.
## Methods

```c#
protected virtual void LayoutScrollbar( ) 
```
Work out how big the scrollbars need to be and layout the current PVS
```c#
void Close( object target) 
```
Close this node
```c#
void ExpandPathTo( object obj) 
```
Expand the path all the way to this object
```c#
void Open( object target) 
```
Open this node
```c#
protected TreeNode ResolveNode( object obj, bool createPath) 
```
Convert from an object to a TreeNode
```c#
void Toggle( object target) 
```
Toggle this node open or closed
```c#
bool TryGetItemRect( object item, out Rect rect) 
```
Try to calculate position and size of a specific item in the tree view.
```c#
protected override string GetTooltip( object obj) 
```
OverridesBaseItemWidget.GetTooltipCalled to retrieve a tooltip for given item.
```c#
override bool IsSelected( object obj) 
```
OverridesBaseItemWidget.IsSelectedReturn true if this item is selected.
```c#
protected override void OnDragHoverItem( DragEvent ev, VirtualWidget item) 
```
OverridesBaseItemWidget.OnDragHoverItemCalled when a dragged item is being hovered over this widget.
This is the place to make drag and drop previews.
```c#
protected override bool OnDragItem( VirtualWidget item) 
```
OverridesBaseItemWidget.OnDragItemCalled when we start to drag an item.
```c#
protected override void OnDropOnItem( DragEvent ev, VirtualWidget item) 
```
OverridesBaseItemWidget.OnDropOnItemCalled when an item is drag and dropped onto this widget.
```c#
protected override void OnItemActivated( object item) 
```
OverridesBaseItemWidget.OnItemActivated
```c#
protected override void OnItemContextMenu( VirtualWidget pressedItem, MouseEvent e) 
```
OverridesBaseItemWidget.OnItemContextMenuThe item has been right clicked
```c#
protected override DropAction OnItemDrag( ItemDragEvent e) 
```
OverridesBaseItemWidget.OnItemDragCalled when a dragged item is being hovered over this widget.
This is the place to make drag and drop previews.
```c#
protected override bool OnItemPressed( VirtualWidget pressedItem, MouseEvent e) 
```
OverridesBaseItemWidget.OnItemPressedAllows over-riding mouse press on an item, without click or selection.
Return true to allow default behavior.
```c#
protected override void OnKeyPressOnItem( KeyEvent e, object item) 
```
OverridesBaseItemWidget.OnKeyPressOnItemA key has been pressed on this selected item.
```c#
protected override void OnPaint( ) 
```
OverridesBaseItemWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
```c#
protected override void OnSelectionAdded( object item) 
```
OverridesBaseItemWidget.OnSelectionAdded
```c#
protected override void PaintItem( VirtualWidget item) 
```
OverridesBaseItemWidget.PaintItem
```c#
protected override void PaintItemDebug( VirtualWidget item) 
```
OverridesBaseItemWidget.PaintItemDebug
```c#
protected override void Rebuild( ) 
```
OverridesBaseItemWidget.RebuildRebuild the panel layout.
```c#
protected override object ResolveObject( object obj) 
```
OverridesBaseItemWidget.ResolveObjectConvert from an object to a TreeNode
```c#
override void ScrollTo( object target) 
```
OverridesBaseItemWidget.ScrollToEnsure that given item is in view, scrolling to it if necessary.
```c#
override bool SelectMoveColumn( int positions) 
```
OverridesBaseItemWidget.SelectMoveColumn
```c#
override bool SelectMoveRow( int positions) 
```
OverridesBaseItemWidget.SelectMoveRow
```c#
override void SetSelected( object obj, bool state, bool skipEvents) 
```
OverridesBaseItemWidget.SetSelectedSet the selected object state. If state is true and ExpandForSelection is true, we'll
try to expand the tree path to the selected object.
## Inheriting Types

