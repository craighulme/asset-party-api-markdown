# TransformControlWidget

## ```c#
Derives from ControlWidget
```

## Summary

OverridesControlWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
## Constructors

```c#
TransformControlWidget( SerializedProperty property) 
```
No Summary
## Methods

```c#
protected override void OnPaint( ) 
```
OverridesControlWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
```c#
protected override Vector2 SizeHint( ) 
```
OverridesControlWidget.SizeHintShould return the size this widget really wants to be if it can its way. The default
is that you don't care - and just to return whatever the base value is.
