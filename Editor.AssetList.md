# AssetList

## Derives from ListView

## Summary

Displays a list of assets, set byBaseItemWidget.SetItems. They should be eitherEditor.Assetor System.IO.DirectoryInfo.
## Constructors

```c#
AssetList( Widget parent) 
```
No Summary
## Fields

```c#
Action<Asset> OnAssetHighlight
```
Asset has been clicked
```c#
Action<Asset> OnAssetSelected
```
Asset has been selected (double click, or enter)
```c#
Action<Asset[]> OnAssetsHighlight
```
Assets has been selected
```c#
Action<DirectoryInfo> OnFolderSelected
```
Asset has been selected (double click, or enter)
```c#
Action<Package> OnPackageHighlight
```
Asset has been clicked
```c#
Action<Package> OnPackageSelected
```
Asset has been selected (double click, or enter)
```c#
Action OnViewModeChanged
```
Called when the viewmode has been modified via user input
## Properties

```c#
AssetBrowser Browser { get; set; } 
```
Link to the owning browser, if we have one.
```c#
int ViewMode { get; } 
```
Current view model.
PAINDAY TODO: This should be an enum, and have a public setter.
## Methods

```c#
void SetIconMode( int iconSize) 
```
Switch the asset list to show icons.
```c#
void SetListMode( ) 
```
Switch the asset list to list mode.
```c#
void SetViewMode( int i) 
```
Set asset list view mode.
```c#
override void OnDragDrop( DragEvent ev) 
```
OverridesBaseItemWidget.OnDragDropSomething was dragged and dropped on this widget. Apply the data here, if its valid.RequiresWidget.AcceptDropsto function.
```c#
override void OnDragHover( DragEvent ev) 
```
OverridesBaseItemWidget.OnDragHoverCursor with drag and drop data moved on this widget.RequiresWidget.AcceptDropsto function.
```c#
protected override void OnDropOnItem( DragEvent ev, VirtualWidget item) 
```
OverridesBaseItemWidget.OnDropOnItemCalled when an item is drag and dropped onto this widget.
```c#
protected override void OnKeyPress( KeyEvent e) 
```
OverridesBaseItemWidget.OnKeyPressA key has been pressed. Your widget needs keyboard focus for this to be called - see FocusMode.
```c#
protected override void OnMouseLeave( ) 
```
OverridesWidget.OnMouseLeaveMouse cursor exited the bounds of this widget.
```c#
protected override void OnWheel( WheelEvent e) 
```
OverridesBaseScrollWidget.OnWheelMouse wheel was scrolled while the mouse cursor was over this widget.
