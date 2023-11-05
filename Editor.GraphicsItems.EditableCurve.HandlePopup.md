# HandlePopup

## Derives from Widget

## Summary

This would be a lot simpler if we just passed the handle to it, and let it fuck with it directly!!
## Constructors

```c#
HandlePopup( Widget parent) 
```
No Summary
## Fields

```c#
bool AimUp
```
No Summary
```c#
FloatProperty X
```
No Summary
```c#
FloatProperty Y
```
No Summary
## Properties

```c#
HandleMode HandleMode { get; set; } 
```
No Summary
## Methods

```c#
protected bool PaintButton( Button b, HandleMode h, string icon) 
```
No Summary
```c#
void UpdateFrom( Handle handle) 
```
No Summary
```c#
protected override void DoLayout( ) 
```
OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
