# FloatingPointProperty<T>

## ```c#
Derives from Widget
```

## Summary

A text box with a draggable icon on the left.
Dragging the icon left and right will change the value
Dragging the icon up and down will change the rate at which the value changes
So dragging down, then left and right will change in 100s, dragging up and then left and right will change in 0.01s
## Type Parameters

```c#
T
```
No Summary
## Constructors

```c#
FloatingPointProperty( Widget parent) 
```
No Summary
```c#
FloatingPointProperty( string label, Widget parent) 
```
No Summary
## Fields

```c#
T _value
```
No Summary
```c#
Color HighlightColor
```
No Summary
## Properties

```c#
float DragValueSpeed { get; set; } 
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
LineEdit LineEdit { get; } 
```
No Summary
```c#
T Value { get; set; } 
```
No Summary
## Methods

```c#
protected virtual void OnDragValue( Decimal add) 
```
No Summary
```c#
protected virtual void TextToValue( ) 
```
No Summary
```c#
protected virtual string ValueToText( string format = null) 
```
No Summary
```c#
protected override void DoLayout( ) 
```
OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
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
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
## Events

```c#
OnValueEdited( ) 
```
No Summary
