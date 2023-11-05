# SegmentedControl

## 
```c#
Derives from Widget
```

## Summary

OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
## Constructors

```c#
SegmentedControl( Widget parent = null) 
```
No Summary
## Fields

```c#
Action<string> OnSelectedChanged
```
No Summary
## Properties

```c#
string Selected { get; } 
```
No Summary
```c#
int SelectedIndex { get; } 
```
No Summary
## Methods

```c#
void AddOption( string name, string icon = null) 
```
No Summary
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
