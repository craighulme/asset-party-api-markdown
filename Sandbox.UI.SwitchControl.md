# SwitchControl

## Derives from BaseControl

## Summary

OverridesPanel.BuildRenderTreeOverridden/implemented by Razor templating to build a render tree.
## Constructors

```c#
SwitchControl( ) 
```
No Summary
## Properties

```c#
RenderFragment Label { get; set; } 
```
No Summary
```c#
Action<bool> OnValueChanged { get; set; } 
```
No Summary
```c#
bool Value { get; set; } 
```
No Summary
## Methods

```c#
protected override void BuildRenderTree( RenderTreeBuilder __builder) 
```
OverridesPanel.BuildRenderTreeOverridden/implemented by Razor templating to build a render tree.
```c#
protected override string GetRenderTreeChecksum( ) 
```
OverridesPanel.GetRenderTreeChecksumOverridden/implemented by Razor templating, contains render tree checksum to determine when the render tree content has changed.
```c#
protected override void OnMouseDown( MousePanelEvent e) 
```
OverridesPanel.OnMouseDownCalled when the player presses down the left or right mouse buttons while hovering this panel.
