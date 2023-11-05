# VrHand

## 
```c#
Derives from ValueType
```

## Summary

Velocity of this hand (degrees/s)
## Properties

```c#
Angles AngularVelocity { get; } 
```
Velocity of this hand (degrees/s)
```c#
DigitalInput ButtonA { get; } 
```
No Summary
```c#
DigitalInput ButtonB { get; } 
```
No Summary
```c#
AnalogInput Grip { get; } 
```
No Summary
```c#
AnalogInput2D Joystick { get; } 
```
No Summary
```c#
DigitalInput JoystickPress { get; } 
```
No Summary
```c#
Transform Transform { get; } 
```
Transform of this hand
```c#
AnalogInput Trigger { get; } 
```
No Summary
```c#
Vector3 Velocity { get; } 
```
Velocity of this hand
## Methods

```c#
float GetFingerCurl( int index) 
```
No Summary
```c#
float GetFingerSplay( int index) 
```
No Summary
```c#
float GetFingerValue( FingerValue value) 
```
No Summary
```c#
void TriggerHapticVibration( float duration, float frequency, float amplitude) 
```
Triggers a haptic vibration event on the controller for this hand.
## Referencing Members

```c#
VrHand = VrInput.LeftHand { get; } 
```
```c#
VrHand = VrInput.RightHand { get; } 
```
