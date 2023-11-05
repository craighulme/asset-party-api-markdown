# DecibelSliderProperty

## 
```c#
Derives from Widget
```

## Summary

A text box with a draggable icon on the left.
Dragging the icon left and right will change the value
Dragging the icon up and down will change the rate at which the value changes
So dragging down, then left and right will change in 100s, dragging up and then left and right will change in 0.01s
## Constructors

```c#
DecibelSliderProperty( Widget parent) 
```
No Summary
## Fields

```c#
static Dictionary<int, string> DecibelNames
```
No Summary
## Properties

```c#
FloatSlider FloatSlider { get; } 
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
float Value { get; set; } 
```
No Summary
## Methods

```c#
string DecibelString( int value) 
```
No Summary
```c#
protected override void DoLayout( ) 
```
OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
```c#
protected override void OnMouseClick( MouseEvent e) 
```
OverridesWidget.OnMouseClickCalled when this widget is left clicked (on mouse release).
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
## Events

```c#
OnValueEdited( ) 
```
No Summary
