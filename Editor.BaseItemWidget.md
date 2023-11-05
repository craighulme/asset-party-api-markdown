# BaseItemWidget

## 
```c#
Derives from BaseScrollWidget
```

## Summary

Called when right clicking on the item's parent.
## Constructors

```c#
BaseItemWidget( Widget parent = null) 
```
No Summary
## Fields

```c#
protected List<object> _items
```
No Summary
```c#
protected HashSet<VirtualWidget> ItemLayouts
```
No Summary
## Properties

```c#
Action BodyContextMenu { get; set; } 
```
Called when right clicking on the item's parent.
```c#
Rect CanvasRect { get; } 
```
The inner of LocalRect with Margin
```c#
ItemDragEvent CurrentItemDragEvent { get; } 
```
No Summary
```c#
Action<object> ItemActivated { get; set; } 
```
Called when an item is double left clicked.
```c#
Action<object> ItemClicked { get; set; } 
```
Called when an item is selected.
```c#
Action<object> ItemContextMenu { get; set; } 
```
Called when an item is right clicked.
```c#
Action<object> ItemDeselected { get; set; } 
```
Called when an item is no longer selected.
```c#
Func<object, bool> ItemDrag { get; set; } 
```
Called to see whether or not we can drag a specific item.
```c#
Action<object> ItemHoverEnter { get; set; } 
```
Called when an item is hovered by the user's cursor.
```c#
Action<object> ItemHoverLeave { get; set; } 
```
Called when an item is no longer hovered by the user's cursor.
```c#
Action<VirtualWidget> ItemPaint { get; set; } 
```
Used to overwrite an item's style
```c#
IEnumerable<object> Items { get; } 
```
No Summary
```c#
Action<object> ItemSelected { get; set; } 
```
Called when an item is selected.
```c#
Action<object[]> ItemsSelected { get; set; } 
```
Multiple items have been selected
```c#
Margin Margin { get; set; } 
```
No Summary
```c#
bool MultiSelect { get; set; } 
```
Whether to allow selecting multiple items at once.
```c#
IEnumerable<object> SelectedItems { get; } 
```
Selected items.
```c#
SelectionSystem Selection { get; set; } 
```
No Summary
```c#
Func<object> SelectionOverride { get; set; } 
```
Can override an item's selection here.
```c#
protected float TimeMsPaint { get; } 
```
No Summary
```c#
protected float timeMsRebuild { get; } 
```
No Summary
```c#
bool ToggleSelect { get; set; } 
```
If set, selecting an item will not deselect all already selected items, clicking a selected item will deselect it.
```c#
override bool ProvidesDebugMode { get; } 
```
OverridesWidget.ProvidesDebugModeIf true then this widget has a debug mode that can be activated
## Methods

```c#
virtual void Clear( ) 
```
Remove all items.
```c#
virtual void Dirty( object dirtyObject = null) 
```
No Summary
```c#
protected virtual string GetTooltip( object obj) 
```
Called to retrieve a tooltip for given item.
```c#
virtual bool IsSelected( object obj) 
```
Return true if this item is selected.
```c#
protected virtual void OnDragHoverItem( DragEvent ev, VirtualWidget item) 
```
Called when a dragged item is being hovered over this widget.
This is the place to make drag and drop previews.
```c#
protected virtual bool OnDragItem( VirtualWidget item) 
```
Called when we start to drag an item.
```c#
protected virtual void OnDropOnItem( DragEvent ev, VirtualWidget item) 
```
Called when an item is drag and dropped onto this widget.
```c#
protected virtual void OnHoverChanged( object oldHover, object newHover) 
```
Hover has changed, neither of these objects are guaranteed to be non null.
```c#
protected virtual void OnItemActivated( object item) 
```
No Summary
```c#
protected virtual void OnItemContextMenu( VirtualWidget pressedItem, MouseEvent e) 
```
The item has been right clicked
```c#
protected virtual DropAction OnItemDrag( ItemDragEvent e) 
```
Called when a dragged item is being hovered over this widget.
This is the place to make drag and drop previews.
```c#
protected virtual bool OnItemPressed( VirtualWidget pressedItem, MouseEvent e) 
```
Allows over-riding mouse press on an item, without click or selection.
Return true to allow default behavior.
```c#
protected virtual void OnKeyPressOnItem( KeyEvent e, object item) 
```
A key has been pressed on this selected item.
```c#
protected virtual void OnLayoutChanged( ) 
```
No Summary
```c#
protected virtual void OnSelectionAdded( object item) 
```
No Summary
```c#
protected virtual void PaintItem( VirtualWidget item) 
```
No Summary
```c#
protected virtual void PaintItemDebug( VirtualWidget item) 
```
No Summary
```c#
protected virtual void Rebuild( ) 
```
Rebuild the panel layout.
```c#
protected virtual object ResolveObject( object obj) 
```
For derived classes where the object is wrapped in another class (i.e. TreeView)
```c#
virtual void ScrollTo( object target) 
```
Ensure that given item is in view, scrolling to it if necessary.
```c#
virtual void ScrollTo( float targetPosition, float height) 
```
Ensure that given position is in view, scrolling to it if necessary.
```c#
virtual bool SelectMoveColumn( int positions) 
```
No Summary
```c#
virtual bool SelectMoveRow( int positions) 
```
No Summary
```c#
virtual void SetSelected( object obj, bool state, bool skipEvents = false) 
```
Set the selection state of an item.
```c#
virtual void UnselectAll( ) 
```
No Summary
```c#
T AddItem<T,>( T item) 
```
Add given item to this widget.
```c#
void AddItems( IEnumerable<object> items) 
```
Add multiple items.
```c#
protected object GetAtIndex( int i) 
```
Returns the item at given index, or null.
```c#
VirtualWidget GetItemAt( Vector2 localPosition) 
```
Get the virtual item at this local position.
```c#
protected int ItemIndex( object item) 
```
Returns the index of given item.
```c#
void RemoveItem( object item) 
```
Remove given item from this widget.
```c#
protected void SelectAll( ) 
```
No Summary
```c#
void SelectItem( object obj, bool add = false, bool skipEvents = false) 
```
Select given item.
```c#
bool SelectMove( int i) 
```
Move the selection pointer by this many positions.
```c#
void SetItems( IEnumerable<object> items) 
```
Set the items in the list.
```c#
void UpdateIfDirty( ) 
```
No Summary
```c#
protected override void OnDoubleClick( MouseEvent e) 
```
OverridesWidget.OnDoubleClickCalled when the widget was double clicked with any mouse button.
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
protected override void OnDragStart( ) 
```
OverridesWidget.OnDragStartCalled when dragging.Widget.IsDraggableshould be true.
```c#
protected override void OnKeyPress( KeyEvent e) 
```
OverridesBaseScrollWidget.OnKeyPressA key has been pressed. Your widget needs keyboard focus for this to be called - see FocusMode.
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
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
```c#
protected override void OnResize( ) 
```
OverridesWidget.OnResizeCalled when the widgets' size was changed.
```c#
protected override void OnScrollChanged( ) 
```
OverridesBaseScrollWidget.OnScrollChangedCalled when the scroll position has changed.
## Nested Types

## Inheriting Types

