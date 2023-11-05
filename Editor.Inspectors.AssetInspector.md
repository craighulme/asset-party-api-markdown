# AssetInspector

## 
```c#
Derives from Widget
```

## Summary

Called when the values of this GameResource are edited
## Constructors

```c#
AssetInspector( Widget parent, Asset target) 
```
No Summary
## Properties

```c#
Asset Asset { get; set; } 
```
No Summary
## Methods

```c#
void UpdateResource( Asset target, GameResource assetObject) 
```
Called when the values of this GameResource are edited
```c#
protected override void DoLayout( ) 
```
OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
```c#
protected override void OnMouseRightClick( MouseEvent e) 
```
OverridesWidget.OnMouseRightClickCalled when this widget is right clicked (on mouse release).
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
## Nested Types

