# CurveEditorToolbar

## 
```c#
Derives from Widget
```

## Summary

A widget which contains an editable curve
## Constructors

```c#
CurveEditorToolbar( Widget parent, CurveEditor editor) 
```
No Summary
## Properties

```c#
Vector2Property TimeRange { get; set; } 
```
No Summary
```c#
Vector2Property ValueRange { get; set; } 
```
No Summary
## Methods

```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
