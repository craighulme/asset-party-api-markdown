# WorldInput

## ```c#
Derives from object
```

## Summary

WorldInput can be used to simulate standard mouse inputs on WorldPanels.
## Remarks

## Constructors

```c#
WorldInput( ) 
```
No Summary
## Properties

```c#
Panel Active { get; } 
```
TheUI.Panelthat is currently pressed by this input.
```c#
bool Enabled { get; set; } 
```
This input won't tick when this is false.
Any hovered panels will be cleared.
```c#
Panel Hovered { get; } 
```
TheUI.Panelthat is currently hovered by this input.
```c#
bool MouseLeftPressed { get; set; } 
```
Simulate if the left mouse button is pressed.
You can useInput.Down.
```c#
bool MouseRightPressed { get; set; } 
```
Simulate if the right mouse button is pressed.
You can useInput.Down.
```c#
float MouseScroll { get; set; } 
```
Simulate the mouse scroll wheel.
You could useInput.MouseWheelOr you could simulate it with the camera view delta for example.
```c#
Ray Ray { get; set; } 
```
The Ray used to intersect with your world panels, simulating mouse position.
```c#
bool UseMouseInput { get; set; } 
```
Instead of simulating mouse input, this will simply use the mouse input.
