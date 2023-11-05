# FloatControlWidget

## ```c#
Derives from StringControlWidget
```

## Summary

If true we can draw a slider
## Constructors

```c#
FloatControlWidget( SerializedProperty property) 
```
No Summary
## Properties

```c#
bool HasRange { get; set; } 
```
If true we can draw a slider
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
Vector2 Range { get; set; } 
```
The range, min and max
```c#
bool RangeClamped { get; set; } 
```
True if the range is clamped between min and max
```c#
float RangeStep { get; set; } 
```
The step size between range
## Methods

```c#
protected virtual void OnDragValue( Decimal add) 
```
No Summary
```c#
protected override void DoLayout( ) 
```
OverridesStringControlWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
```c#
protected override void OnMouseMove( MouseEvent e) 
```
OverridesWidget.OnMouseMoveCalled when the mouse cursor is moved while being over this widget.
```c#
protected override void OnMousePress( MouseEvent e) 
```
OverridesWidget.OnMousePressCalled when mouse is pressed over this widget.
```c#
protected override void OnMouseReleased( MouseEvent e) 
```
OverridesWidget.OnMouseReleasedCalled when mouse is released over this widget.
```c#
protected override void OnValueChanged( ) 
```
OverridesStringControlWidget.OnValueChanged
```c#
protected override void PaintControl( ) 
```
OverridesControlWidget.PaintControl
```c#
protected override object StringToValue( string text) 
```
OverridesStringControlWidget.StringToValue
```c#
protected override string ValueToString( ) 
```
OverridesStringControlWidget.ValueToString
## Inheriting Types

