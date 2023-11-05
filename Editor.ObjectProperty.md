# ObjectProperty

## 
```c#
Derives from Widget
```

## Summary

OverridesWidget.OnMouseClickCalled when this widget is left clicked (on mouse release).
## Constructors

```c#
ObjectProperty( Widget parent, Type type) 
```
No Summary
## Properties

```c#
Type TargetType { get; set; } 
```
No Summary
```c#
object Value { get; set; } 
```
No Summary
## Methods

```c#
static bool IsApplicable( Type type) 
```
No Summary
```c#
void SetValue( object value) 
```
No Summary
```c#
protected override void OnMouseClick( MouseEvent e) 
```
OverridesWidget.OnMouseClickCalled when this widget is left clicked (on mouse release).
```c#
protected override void OnMousePress( MouseEvent e) 
```
OverridesWidget.OnMousePressCalled when mouse is pressed over this widget.
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
