# MouseButtons

## Derives from Enum

## Summary

State of mouse buttons being pressed or not.
## Fields

```c#
static MouseButtons Back = 8
```
The "back" mouse button (mouse4) being pressed in.
```c#
static MouseButtons Forward = 16
```
The "forward" mouse button (mouse5) being pressed in.
```c#
static MouseButtons Left = 1
```
Left mouse button is being pressed.
```c#
static MouseButtons Middle = 4
```
Middle mouse button (mouse wheel) is being pressed in.
```c#
static MouseButtons None = 0
```
No buttons are being pressed.
```c#
static MouseButtons Right = 2
```
Right mouse button is being pressed.
## Referencing Members

```c#
MouseButtons = MouseEvent.Button { get; } 
```
```c#
MouseButtons = GraphicsMouseEvent.Button { get; } 
```
```c#
MouseButtons = GraphicsMouseEvent.Buttons { get; } 
```
```c#
MouseButtons = MouseEvent.ButtonState { get; } 
```
```c#
MouseButtons = MousePanelEvent.MouseButton { get; set; } 
```
```c#
static MouseButtons = Application.MouseButtons { get; } 
```
```c#
void WebSurface.TellMouseButton( MouseButtons, bool ) 
```
