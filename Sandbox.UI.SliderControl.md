# SliderControl

## 
```c#
Derives from BaseControl
```

## Summary

The right side of the slider.
## Constructors

```c#
SliderControl( ) 
```
No Summary
```c#
SliderControl( float min, float max, float step = 1) 
```
No Summary
## Properties

```c#
float Max { get; set; } 
```
The right side of the slider.
```c#
float Min { get; set; } 
```
The left side of the slider.
```c#
string NumberFormat { get; set; } 
```
How to display numbers in this control
```c#
Action<float> OnValueChanged { get; set; } 
```
No Summary
```c#
bool ShowRange { get; set; } 
```
Show the range values above the slider
```c#
bool ShowTextEntry { get; set; } 
```
When changing the value show the tooltip
```c#
bool ShowValueTooltip { get; set; } 
```
When changing the value show the tooltip
```c#
float Step { get; set; } 
```
If set to 1, value will be rounded to 1's
If set to 10, value will be rounded to 10's
If set to 0.1, value will be rounded to 0.1's
```c#
float Value { get; set; } 
```
No Summary
## Methods

```c#
virtual float ScreenPosToValue( Vector2 pos) 
```
Convert a screen position to a value. The value is clamped, but not snapped.
```c#
protected override void BuildRenderTree( RenderTreeBuilder __builder) 
```
OverridesPanel.BuildRenderTreeOverridden/implemented by Razor templating to build a render tree.
```c#
protected override string GetRenderTreeChecksum( ) 
```
OverridesPanel.GetRenderTreeChecksumOverridden/implemented by Razor templating, contains render tree checksum to determine when the render tree content has changed.
```c#
protected override void OnMiddleClick( MousePanelEvent e) 
```
OverridesPanel.OnMiddleClickCalled when the player releases their middle mouse button (Mouse 3) while hovering this panel.
```c#
protected override void OnMouseDown( MousePanelEvent e) 
```
OverridesPanel.OnMouseDownOn mouse press jump to that position
```c#
protected override void OnMouseMove( MousePanelEvent e) 
```
OverridesPanel.OnMouseMoveIf we move the mouse while we're being pressed then set the value
