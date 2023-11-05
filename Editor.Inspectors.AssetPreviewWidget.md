# AssetPreviewWidget

## 
```c#
Derives from NativeRenderingWidget
```

## Summary

OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
## Constructors

```c#
AssetPreviewWidget( Widget parent) 
```
No Summary
## Properties

```c#
Asset Asset { set; } 
```
No Summary
```c#
bool EnableFlatMaterial { get; set; } 
```
No Summary
```c#
bool EnableGrid { get; set; } 
```
No Summary
```c#
bool EnablePostProcessing { get; set; } 
```
No Summary
```c#
bool EnableShadows { get; set; } 
```
No Summary
```c#
bool EnableWireFrame { get; set; } 
```
No Summary
## Methods

```c#
void OpenSettings( ) 
```
No Summary
```c#
protected override void DoLayout( ) 
```
OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
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
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
```c#
protected override void OnWheel( WheelEvent e) 
```
OverridesWidget.OnWheelMouse wheel was scrolled while the mouse cursor was over this widget.
```c#
override void PreFrame( ) 
```
OverridesNativeRenderingWidget.PreFrame
