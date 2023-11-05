# BodyGroupsControlWidget

## Derives from ControlWidget

## Summary

OverridesControlWidget.ValueHash
## Constructors

```c#
BodyGroupsControlWidget( SerializedProperty property) 
```
No Summary
## Properties

```c#
protected override int ValueHash { get; } 
```
OverridesControlWidget.ValueHash
## Methods

```c#
void Rebuild( ) 
```
No Summary
```c#
protected override void OnPaint( ) 
```
OverridesControlWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
```c#
protected override void OnValueChanged( ) 
```
OverridesControlWidget.OnValueChanged
```c#
protected override Vector2 SizeHint( ) 
```
OverridesControlWidget.SizeHintShould return the size this widget really wants to be if it can its way. The default
is that you don't care - and just to return whatever the base value is.
