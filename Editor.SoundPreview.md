# SoundPreview

## ```c#
Derives from Widget
```

## Summary

OverridesQObject.OnDestroyed
## Constructors

```c#
SoundPreview( Widget parent) 
```
No Summary
## Properties

```c#
Asset Asset { get; set; } 
```
No Summary
```c#
float Distance { get; } 
```
No Summary
## Methods

```c#
void Tick( ) 
```
No Summary
```c#
override void OnDestroyed( ) 
```
OverridesQObject.OnDestroyed
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
