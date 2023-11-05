# CurveEditorPopup

## ```c#
Derives from PopupWidget
```

## Summary

OverridesWidget.OnMouseMoveCalled when the mouse cursor is moved while being over this widget.
## Constructors

```c#
CurveEditorPopup( Widget parent, Curve value) 
```
No Summary
## Properties

```c#
Action<Curve> OnValueChanged { get; set; } 
```
No Summary
```c#
Curve Value { get; set; } 
```
No Summary
## Methods

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
