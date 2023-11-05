# InputMotionData

## Derives from ValueType

## Summary

Represents the current state of a device's motion sensor(s).
## Fields

```c#
Vector3 AngularVelocity
```
Angular velocity
```c#
Vector3 PositionalAcceleration
```
Positional acceleration
```c#
Rotation Rotation
```
Sensor-fused absolute rotation (will drift in heading)
## Referencing Members

```c#
static InputMotionData = Input.MotionData { get; } 
```
