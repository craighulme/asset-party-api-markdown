# ToggleSwitch

## 
```c#
Derives from Widget
```

## Summary

OverridesWidget.OnMouseClickCalled when this widget is left clicked (on mouse release).
## Constructors

```c#
ToggleSwitch( string text, Widget parent = null) 
```
No Summary
## Properties

```c#
string Text { get; set; } 
```
No Summary
```c#
bool Value { get; set; } 
```
No Summary
## Methods

```c#
protected override void OnMouseClick( MouseEvent e) 
```
OverridesWidget.OnMouseClickCalled when this widget is left clicked (on mouse release).
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
```c#
protected override Vector2 SizeHint( ) 
```
OverridesWidget.SizeHintShould return the size this widget really wants to be if it can its way. The default
is that you don't care - and just to return whatever the base value is.
