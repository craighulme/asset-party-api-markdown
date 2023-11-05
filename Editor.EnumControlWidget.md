# EnumControlWidget

## ```c#
Derives from ControlWidget
```

## Summary

If true, then this control is operating in flags mode (FlagsAttribute)
## Constructors

```c#
EnumControlWidget( SerializedProperty property) 
```
No Summary
## Properties

```c#
bool IsFlagsMode { get; init; } 
```
If true, then this control is operating in flags mode (FlagsAttribute)
```c#
override bool IsControlButton { get; } 
```
OverridesControlWidget.IsControlButton
```c#
override bool IsControlHovered { get; } 
```
OverridesControlWidget.IsControlHovered
## Methods

```c#
protected override void OnMousePress( MouseEvent e) 
```
OverridesWidget.OnMousePressCalled when mouse is pressed over this widget.
```c#
protected override void PaintControl( ) 
```
OverridesControlWidget.PaintControl
