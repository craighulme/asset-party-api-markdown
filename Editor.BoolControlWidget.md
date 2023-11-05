# BoolControlWidget

## Derives from ControlWidget

## Summary

OverridesWidget.OnDoubleClickCalled when the widget was double clicked with any mouse button.
## Constructors

```c#
BoolControlWidget( SerializedProperty property) 
```
No Summary
## Methods

```c#
protected override void OnDoubleClick( MouseEvent e) 
```
OverridesWidget.OnDoubleClickCalled when the widget was double clicked with any mouse button.
```c#
protected override void OnMousePress( MouseEvent e) 
```
OverridesWidget.OnMousePressCalled when mouse is pressed over this widget.
```c#
protected override void OnPaint( ) 
```
OverridesControlWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
```c#
protected override Vector2 SizeHint( ) 
```
OverridesControlWidget.SizeHintShould return the size this widget really wants to be if it can its way. The default
is that you don't care - and just to return whatever the base value is.
