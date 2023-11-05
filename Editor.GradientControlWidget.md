# GradientControlWidget

## 
```c#
Derives from ControlWidget
```

## Summary

OverridesWidget.OnMouseReleasedCalled when mouse is released over this widget.
## Constructors

```c#
GradientControlWidget( SerializedProperty property) 
```
No Summary
## Methods

```c#
protected override void OnMouseReleased( MouseEvent e) 
```
OverridesWidget.OnMouseReleasedCalled when mouse is released over this widget.
```c#
protected override void PaintOver( ) 
```
OverridesControlWidget.PaintOver
```c#
protected override Vector2 SizeHint( ) 
```
OverridesControlWidget.SizeHintShould return the size this widget really wants to be if it can its way. The default
is that you don't care - and just to return whatever the base value is.
