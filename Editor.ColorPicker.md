# ColorPicker

## ```c#
Derives from Widget
```

## Summary

A color picker widget that makes it easy to select or edit colors
## Constructors

```c#
ColorPicker( Widget parent = null, Color startColor = null) 
```
No Summary
## Properties

```c#
float Alpha { get; set; } 
```
No Summary
```c#
float Hue { get; set; } 
```
No Summary
```c#
bool IsHDR { get; set; } 
```
No Summary
```c#
float Range { get; set; } 
```
No Summary
```c#
Color Value { get; set; } 
```
The current color value
```c#
Action<Color> ValueChanged { get; set; } 
```
No Summary
```c#
Color ValueWithoutRange { get; } 
```
No Summary
## Methods

```c#
static void OpenColorPopup( Color color, Action<Color> onChange) 
```
No Summary
```c#
protected virtual void PaintHandle( Rect rect, float pos) 
```
No Summary
```c#
override void ChildValuesChanged( Widget source) 
```
OverridesWidget.ChildValuesChanged
```c#
protected override void DoLayout( ) 
```
OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
```c#
protected override void Signal( WidgetSignal signal) 
```
OverridesWidget.Signal
