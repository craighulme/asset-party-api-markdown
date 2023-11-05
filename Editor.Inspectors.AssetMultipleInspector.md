# AssetMultipleInspector

## 
```c#
Derives from Widget
```

## Summary

OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
## Constructors

```c#
AssetMultipleInspector( Widget parent, Asset[] targets) 
```
No Summary
## Properties

```c#
Asset[] Assets { get; set; } 
```
No Summary
## Methods

```c#
protected override void DoLayout( ) 
```
OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
