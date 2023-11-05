# WebPanel

## ```c#
Derives from Panel
```

## Summary

A panel that displays an interactive web page.
## Constructors

```c#
WebPanel( ) 
```
No Summary
## Properties

```c#
WebSurface Surface { get; } 
```
Access to the HTML surface to change URL, etc.
## Methods

```c#
protected override void OnBlur( PanelEvent e) 
```
OverridesPanel.OnBlurCalled when this panel loses input focus.
```c#
override void OnButtonEvent( ButtonEvent e) 
```
OverridesPanel.OnButtonEventCalled when any button, mouse (except for mouse4/5) and keyboard, are pressed or depressed while hovering this panel.
```c#
override void OnDeleted( ) 
```
OverridesPanel.OnDeletedCalled when the panel is about to be deleted.
```c#
protected override void OnFocus( PanelEvent e) 
```
OverridesPanel.OnFocusCalled when this panel receives input focus.
```c#
override void OnKeyTyped( Char k) 
```
OverridesPanel.OnKeyTypedCalled when a printable character has been typed (pressed) while this panel has input focus. (Panel.Focus)
```c#
override void OnLayout( ref Rect layoutRect) 
```
OverridesPanel.OnLayoutThis panel has just been laid out. You can modify its position now and it will affect its children.
This is a useful place to restrict shit to the screen etc.
```c#
protected override void OnMouseDown( MousePanelEvent e) 
```
OverridesPanel.OnMouseDownCalled when the player presses down the left or right mouse buttons while hovering this panel.
```c#
protected override void OnMouseMove( MousePanelEvent e) 
```
OverridesPanel.OnMouseMoveCalled when the cursor moves while hovering this panel.
```c#
protected override void OnMouseUp( MousePanelEvent e) 
```
OverridesPanel.OnMouseUpCalled when the player releases left or right mouse button.
```c#
override void OnMouseWheel( float value) 
```
OverridesPanel.OnMouseWheelCalled when the player scrolls their mouse wheel while hovering this panel.
