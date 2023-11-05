# ButtonState

## ```c#
Derives from ValueType
```

## Summary

Can be used with [ClientInput] for button inputs where you need to know if it was previously down or not.
## Properties

```c#
bool IsDown { get; set; } 
```
Is this button currently down?
```c#
bool Pressed { get; } 
```
Was this button just pressed.
```c#
bool Released { get; } 
```
Was this button just released.
```c#
bool WasDown { get; } 
```
Was this button down previously?
## Operators

```c#
implicit ButtonState =( bool value) 
```
No Summary
