# AssetLocations

## 
```c#
Derives from TreeView
```

## Summary

Called when a "filter" is selected, i.e. "@recent" or "t:vmdl".
## Constructors

```c#
AssetLocations( AssetBrowser parent) 
```
No Summary
## Fields

```c#
Action<string> OnFilterSelected
```
Called when a "filter" is selected, i.e. "@recent" or "t:vmdl".
```c#
Action<DirectoryInfo> OnFolderSelected
```
Called when a folder is selected.
## Methods

```c#
protected override void OnDragHoverItem( DragEvent ev, VirtualWidget item) 
```
OverridesTreeView.OnDragHoverItemCalled when a dragged item is being hovered over this widget.
This is the place to make drag and drop previews.
```c#
protected override void OnDropOnItem( DragEvent ev, VirtualWidget item) 
```
OverridesTreeView.OnDropOnItemCalled when an item is drag and dropped onto this widget.
```c#
protected override void OnPaint( ) 
```
OverridesTreeView.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
```c#
override void SetSelected( object obj, bool state, bool skipEvents) 
```
OverridesTreeView.SetSelectedSet the selected object state. If state is true and ExpandForSelection is true, we'll
try to expand the tree path to the selected object.
