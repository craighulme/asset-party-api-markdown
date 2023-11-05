# MatrixButton

## 
```c#
Derives from Widget
```

## Summary

OverridesWidget.OnMouseEnterMouse cursor entered the bounds of this widget.
## Constructors

```c#
MatrixButton( CollisionMatrixWidget parent, string left, string right) 
```
No Summary
## Properties

```c#
string Left { get; set; } 
```
No Summary
```c#
string Right { get; set; } 
```
No Summary
## Methods

```c#
protected override void OnMouseEnter( ) 
```
OverridesWidget.OnMouseEnterMouse cursor entered the bounds of this widget.
```c#
protected override void OnMouseLeave( ) 
```
OverridesWidget.OnMouseLeaveMouse cursor exited the bounds of this widget.
```c#
protected override void OnMousePress( MouseEvent e) 
```
OverridesWidget.OnMousePressCalled when mouse is pressed over this widget.
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
