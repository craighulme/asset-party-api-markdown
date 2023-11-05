# ListView

## Derives from BaseItemWidget

## Summary

Work out how big the scrollbars need to be and layout the current PVS
## Constructors

```c#
ListView( Widget parent = null) 
```
No Summary
## Properties

```c#
Align ItemAlign { get; set; } 
```
No Summary
```c#
Vector2 ItemSize { get; set; } 
```
No Summary
```c#
Vector2 ItemSpacing { get; set; } 
```
No Summary
## Methods

```c#
protected virtual void LayoutItems( ) 
```
No Summary
```c#
protected virtual void LayoutScrollbar( ) 
```
Work out how big the scrollbars need to be and layout the current PVS
```c#
protected override void OnLayoutChanged( ) 
```
OverridesBaseItemWidget.OnLayoutChanged
```c#
protected override void OnPaint( ) 
```
OverridesBaseItemWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
```c#
protected override void Rebuild( ) 
```
OverridesBaseItemWidget.RebuildRebuild the scrollbars and layout for the visible items
```c#
override void ScrollTo( object target) 
```
OverridesBaseItemWidget.ScrollToEnsure that given item is in view, scrolling to it if necessary.
```c#
override bool SelectMoveRow( int positions) 
```
OverridesBaseItemWidget.SelectMoveRow
## Inheriting Types

