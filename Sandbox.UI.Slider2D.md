# Slider2D

## ```c#
Derives from Panel
```

## Summary

A 2-dimensional slider.
## Constructors

```c#
Slider2D( ) 
```
No Summary
## Fields

```c#
protected Vector2 _value
```
Raw internal value.
## Properties

```c#
Panel Thumb { get; protected set; } 
```
The draggable slider thumb panel.
```c#
Panel Track { get; protected set; } 
```
The background panel.
```c#
Vector2 Value { get; set; } 
```
The actual value. Setting the value will snap and clamp it.
## Methods

```c#
virtual Vector2 ScreenPositionToValue( Vector2 pos) 
```
Convert a screen position to a value. The value is clamped, but not snapped.
```c#
protected override void OnMouseDown( MousePanelEvent e) 
```
OverridesPanel.OnMouseDownOn mouse press jump to that position
```c#
protected override void OnMouseMove( MousePanelEvent e) 
```
OverridesPanel.OnMouseMoveIf we move the mouse while we're being pressed then set the position,
but skip transitions.
```c#
override void SetProperty( string name, string value) 
```
OverridesPanel.SetPropertySet a property on the panel, such as special properties (class,id,styleandvalue, etc.) and properties of the panel's C# class.
