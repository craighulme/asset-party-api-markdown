# GradientEditorWidget

## Derives from Widget

## Summary

The current color value
## Constructors

```c#
GradientEditorWidget( Widget parent = null) 
```
No Summary
## Properties

```c#
protected float AlphaValue { get; set; } 
```
No Summary
```c#
protected Color ColorValue { get; set; } 
```
No Summary
```c#
Gradient Value { get; set; } 
```
The current color value
```c#
Action<Gradient> ValueChanged { get; set; } 
```
No Summary
## Methods

```c#
static void OpenPopup( Widget parent, Gradient input, Action<Gradient> onChange) 
```
Open a gradient editor popup
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
