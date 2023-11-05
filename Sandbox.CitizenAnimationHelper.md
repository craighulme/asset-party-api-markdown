# CitizenAnimationHelper

## ```c#
Derives from ValueType
```

## Summary

A struct to help you set up your citizen based animations
## Constructors

```c#
CitizenAnimationHelper( AnimatedEntity entity) 
```
No Summary
## Properties

```c#
Rotation AimAngle { set; } 
```
No Summary
```c#
float AimBodyWeight { get; set; } 
```
No Summary
```c#
float AimEyesWeight { get; set; } 
```
No Summary
```c#
float AimHeadWeight { get; set; } 
```
No Summary
```c#
float DuckLevel { get; set; } 
```
No Summary
```c#
float FootShuffle { get; set; } 
```
No Summary
```c#
Hand Handedness { get; set; } 
```
No Summary
```c#
HoldTypes HoldType { get; set; } 
```
No Summary
```c#
bool IsClimbing { get; set; } 
```
No Summary
```c#
bool IsGrounded { get; set; } 
```
No Summary
```c#
bool IsNoclipping { get; set; } 
```
No Summary
```c#
bool IsSitting { get; set; } 
```
No Summary
```c#
bool IsSwimming { get; set; } 
```
No Summary
```c#
bool IsWeaponLowered { get; set; } 
```
No Summary
```c#
MoveStyles MoveStyle { get; set; } 
```
We can force the model to walk or run, or let it decide based on the speed.
```c#
float VoiceLevel { get; set; } 
```
No Summary
## Methods

```c#
void TriggerDeploy( ) 
```
No Summary
```c#
void TriggerJump( ) 
```
No Summary
```c#
void WithLookAt( Vector3 look, float eyesWeight = 1, float headWeight = 1, float bodyWeight = 1) 
```
Have the player look at this point in the world
```c#
void WithVelocity( Vector3 Velocity) 
```
No Summary
```c#
void WithWishVelocity( Vector3 Velocity) 
```
No Summary
## Nested Types

## Referencing Members

```c#
virtual void BaseCarriable.SimulateAnimator( CitizenAnimationHelper ) 
```
