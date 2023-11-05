# CurveControlWidget

## Derives from ControlWidget

## Summary

OverridesWidget.OnMousePressCalled when mouse is pressed over this widget.
## Constructors

```c#
CurveControlWidget( SerializedProperty property) 
```
No Summary
## Fields

```c#
Color HighlightColor
```
No Summary
## Methods

```c#
protected override void OnMousePress( MouseEvent e) 
```
OverridesWidget.OnMousePressCalled when mouse is pressed over this widget.
```c#
protected override void PaintOver( ) 
```
OverridesControlWidget.PaintOver
```c#
protected override Vector2 SizeHint( ) 
```
OverridesControlWidget.SizeHintShould return the size this widget really wants to be if it can its way. The default
is that you don't care - and just to return whatever the base value is.
