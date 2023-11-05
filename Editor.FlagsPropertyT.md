# FlagsProperty<T>

## Derives from PropertyEditorWidget
Implements IEditorAttribute<FlagsAttribute>, IEditorAttribute<BitFlagsAttribute>

## Summary

ImplementsIEditorAttribute<T>.SetEditorAttribute
## Type Parameters

```c#
T
```
No Summary
## Constructors

```c#
FlagsProperty( Widget parent) 
```
No Summary
## Fields

```c#
T _value
```
No Summary
## Properties

```c#
T Value { get; set; } 
```
No Summary
## Methods

```c#
protected virtual void OnItemChanged( ) 
```
No Summary
```c#
virtual void SetEditorAttribute( FlagsAttribute attribute) 
```
ImplementsIEditorAttribute<T>.SetEditorAttribute
```c#
virtual void SetEditorAttribute( BitFlagsAttribute attribute) 
```
ImplementsIEditorAttribute<T>.SetEditorAttribute
```c#
protected void OpenMenu( ) 
```
No Summary
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
