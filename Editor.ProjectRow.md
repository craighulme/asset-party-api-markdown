# ProjectRow

## 
```c#
Derives from ItemRow
```

## Summary

Get an auto generated icon for given tag.
## Constructors

```c#
ProjectRow( LocalProject project, Widget parent) 
```
No Summary
## Fields

```c#
protected ContextMenu menu
```
No Summary
## Properties

```c#
protected Package Package { get; set; } 
```
No Summary
```c#
protected LocalProject Project { get; } 
```
No Summary
## Methods

```c#
static Pixmap GetProjectIcon( LocalProject proj, Rect size) 
```
Get an auto generated icon for given tag.
```c#
protected Task UpdatePackageAsync( ) 
```
No Summary
```c#
protected override void CreateUI( ) 
```
OverridesItemRow.CreateUI
```c#
protected override List<InfoItem> GetInfo( ) 
```
OverridesItemRow.GetInfo
```c#
protected override bool IsDisabled( ) 
```
OverridesItemRow.IsDisabled
```c#
override void OnClick( ) 
```
OverridesItemRow.OnClick
```c#
protected override void OnContextMenu( ContextMenuEvent e) 
```
OverridesWidget.OnContextMenuCalled afterWidget.OnMouseRightClick, for the purposes of opening a context menu.
```c#
protected override void OnPaintIcon( Rect iconRect) 
```
OverridesItemRow.OnPaintIcon
## Inheriting Types

