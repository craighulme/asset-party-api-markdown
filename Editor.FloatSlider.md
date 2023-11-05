# FloatSlider

## 
```c#
Implements IEditorAttribute<MinMaxAttribute>, IEditorAttribute<RangeAttribute>
```

## Summary

ImplementsIEditorAttribute<T>.SetEditorAttribute
## Constructors

```c#
FloatSlider( Widget parent) 
```
No Summary
## Properties

```c#
float DeltaValue { get; set; } 
```
No Summary
```c#
Color HighlightColor { get; set; } 
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
Action OnValueEdited { get; set; } 
```
No Summary
```c#
Action<Rect, float> SliderPaint { get; set; } 
```
No Summary
```c#
float Step { get; set; } 
```
No Summary
```c#
float Value { get; set; } 
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
protected override void OnMouseEnter( ) 
```
OverridesWidget.OnMouseEnterMouse cursor entered the bounds of this widget.
```c#
protected override void OnMouseLeave( ) 
```
OverridesWidget.OnMouseLeaveMouse cursor exited the bounds of this widget.
```c#
protected override void OnMouseMove( MouseEvent e) 
```
OverridesWidget.OnMouseMoveCalled when the mouse cursor is moved while being over this widget.
```c#
protected override void OnMousePress( MouseEvent e) 
```
OverridesWidget.OnMousePressCalled when mouse is pressed over this widget.
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
