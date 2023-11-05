# ColorProperty

## Derives from Widget

## Summary

OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
## Constructors

```c#
ColorProperty( Widget parent) 
```
No Summary
## Properties

```c#
bool IsHDR { get; set; } 
```
No Summary
```c#
Color Value { get; set; } 
```
No Summary
## Methods

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
protected override void OnMouseMove( MouseEvent e) 
```
OverridesWidget.OnMouseMoveCalled when the mouse cursor is moved while being over this widget.
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
