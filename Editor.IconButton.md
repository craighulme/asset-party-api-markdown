# IconButton

## Derives from Widget

## Summary

OverridesWidget.OnMouseClickCalled when this widget is left clicked (on mouse release).
## Constructors

```c#
IconButton( string icon, Action onClick = null, Widget parent = null) 
```
No Summary
## Properties

```c#
string Icon { get; set; } 
```
No Summary
```c#
Action OnClick { get; set; } 
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
