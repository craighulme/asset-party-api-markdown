# ActiveGameRow

## 
```c#
Derives from ProjectRow
```

## Summary

This is the variant of ProjectRow we'll show in the Explorer tab.
You shouldn't be able to do too much with this - it's just an indicator
of what the active project is.
## Constructors

```c#
ActiveGameRow( LocalProject project, Widget parent) 
```
No Summary
## Methods

```c#
protected override void CreateUI( ) 
```
OverridesProjectRow.CreateUI
```c#
protected override List<InfoItem> GetInfo( ) 
```
OverridesProjectRow.GetInfo
```c#
override void OnClick( ) 
```
OverridesProjectRow.OnClick
```c#
protected override void OnContextMenu( ContextMenuEvent e) 
```
OverridesProjectRow.OnContextMenuCalled afterWidget.OnMouseRightClick, for the purposes of opening a context menu.
