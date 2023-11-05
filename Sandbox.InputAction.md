# InputAction

## Derives from object

## Summary

An input action defined by a game project.
## Constructors

```c#
InputAction( string name, string keyboardCode, GamepadCode gamepadCode = 0) 
```
No Summary
```c#
InputAction( ) 
```
No Summary
## Properties

```c#
GamepadCode GamepadCode { get; set; } 
```
What gamepad button should this action map to?
```c#
string GroupName { get; set; } 
```
A group name for this input when showing in a binding system
```c#
string KeyboardCode { get; set; } 
```
The key or key combo we'll be watching for.
```c#
string Name { get; set; } 
```
The name of the input action. Used by Input.Down|Pressed|Released.
