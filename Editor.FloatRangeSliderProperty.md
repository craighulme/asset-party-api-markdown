# FloatRangeSliderProperty

## Derives from PropertyEditorWidget
Implements IEditorAttribute< MinMaxAttribute>, IEditorAttribute< RangeAttribute>

## Summary

This is primarily used forEditor.RangedFloatSliderProperty.
## Constructors

```c#
FloatRangeSliderProperty( Widget parent) 
```
No Summary
```c#
FloatRangeSliderProperty( string label, Widget parent) 
```
No Summary
## Properties

```c#
FloatRangeSlider FloatSlider { get; } 
```
No Summary
```c#
string Format { get; set; } 
```
No Summary
```c#
Color HighlightColor { get; set; } 
```
No Summary
```c#
string Icon { get; set; } 
```
No Summary
```c#
string Label { get; set; } 
```
No Summary
```c#
LineEdit LineEditMax { get; } 
```
No Summary
```c#
LineEdit LineEditMin { get; } 
```
No Summary
```c#
float Maximum { get; set; } 
```
No Summary
```c#
float Minimum { get; set; } 
```
No Summary
```c#
float Step { get; set; } 
```
No Summary
```c#
Vector2 Value { get; set; } 
```
No Summary
## Methods

```c#
virtual void SetEditorAttribute( MinMaxAttribute attribute) 
```
ImplementsIEditorAttribute<T>.SetEditorAttribute
```c#
virtual void SetEditorAttribute( RangeAttribute attribute) 
```
ImplementsIEditorAttribute<T>.SetEditorAttribute
```c#
protected override void DoLayout( ) 
```
OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
## Events

```c#
OnValueEdited( ) 
```
No Summary
