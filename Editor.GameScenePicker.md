# GameScenePicker

## 
```c#
Derives from Widget
```

## Summary

Opens an invisible popup above the game screen which allows you to left click once on the scene.
This is great for things like selecting something from the game scene.
## Constructors

```c#
GameScenePicker( ) 
```
No Summary
## Properties

```c#
Action Destroyed { get; set; } 
```
No Summary
## Methods

```c#
protected override void DoLayout( ) 
```
OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
```c#
override void OnDestroyed( ) 
```
OverridesQObject.OnDestroyed
```c#
protected override void OnMouseMove( MouseEvent e) 
```
OverridesWidget.OnMouseMoveCalled when the mouse cursor is moved while being over this widget.
```c#
protected override void OnMouseReleased( MouseEvent e) 
```
OverridesWidget.OnMouseReleasedCalled when mouse is released over this widget.
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
