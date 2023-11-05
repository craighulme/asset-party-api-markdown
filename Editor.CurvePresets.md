# CurvePresets

## 
```c#
Derives from ListView
```

## Summary

A widget which holds a list of user curve presets, saved in a cookie
## Constructors

```c#
CurvePresets( Widget parent, string cookie = "CurvePresets") 
```
No Summary
## Properties

```c#
Func<Curve?> GetCurveToSave { get; set; } 
```
No Summary
```c#
Action<Curve> OnCurveClicked { get; set; } 
```
No Summary
## Methods

```c#
void OnItemClicked( object value) 
```
No Summary
```c#
protected override void OnPaint( ) 
```
OverridesListView.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
```c#
protected override void PaintItem( VirtualWidget item) 
```
OverridesBaseItemWidget.PaintItem
