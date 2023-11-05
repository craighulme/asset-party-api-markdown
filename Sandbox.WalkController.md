# WalkController

## ```c#
Derives from BasePlayerController
```

## Summary

Add our wish direction and speed onto our velocity
## Constructors

```c#
WalkController( ) 
```
No Summary
## Fields

```c#
Duck Duck
```
No Summary
```c#
protected Vector3 maxs
```
No Summary
```c#
protected Vector3 mins
```
No Summary
```c#
protected float SurfaceFriction
```
No Summary
```c#
Unstuck Unstuck
```
No Summary
## Properties

```c#
float Acceleration { get; set; } 
```
No Summary
```c#
float AirAcceleration { get; set; } 
```
No Summary
```c#
float AirControl { get; set; } 
```
No Summary
```c#
bool AutoJump { get; set; } 
```
No Summary
```c#
float BodyGirth { get; set; } 
```
No Summary
```c#
float BodyHeight { get; set; } 
```
No Summary
```c#
float Bounce { get; set; } 
```
No Summary
```c#
float DefaultSpeed { get; set; } 
```
No Summary
```c#
float DistEpsilon { get; set; } 
```
No Summary
```c#
float EyeHeight { get; set; } 
```
No Summary
```c#
float FallSoundZ { get; set; } 
```
No Summary
```c#
float Gravity { get; set; } 
```
No Summary
```c#
float GroundAngle { get; set; } 
```
No Summary
```c#
float GroundFriction { get; set; } 
```
No Summary
```c#
float MaxNonJumpVelocity { get; set; } 
```
No Summary
```c#
float MoveFriction { get; set; } 
```
No Summary
```c#
float Size { get; set; } 
```
No Summary
```c#
float SprintSpeed { get; set; } 
```
No Summary
```c#
float StepSize { get; set; } 
```
No Summary
```c#
float StopSpeed { get; set; } 
```
No Summary
```c#
bool Swimming { get; set; } 
```
No Summary
```c#
float WalkSpeed { get; set; } 
```
No Summary
## Methods

```c#
virtual void Accelerate( Vector3 wishdir, float wishspeed, float speedLimit, float acceleration) 
```
Add our wish direction and speed onto our velocity
```c#
virtual void AirMove( ) 
```
No Summary
```c#
virtual void ApplyFriction( float frictionAmount = 1) 
```
Remove ground friction from velocity
```c#
virtual void CategorizePosition( bool bStayOnGround) 
```
No Summary
```c#
virtual void CheckJumpButton( ) 
```
No Summary
```c#
virtual void CheckLadder( ) 
```
No Summary
```c#
virtual void ClearGroundEntity( ) 
```
We're no longer on the ground, remove it
```c#
virtual float GetWishSpeed( ) 
```
No Summary
```c#
virtual void LadderMove( ) 
```
No Summary
```c#
virtual void Move( ) 
```
No Summary
```c#
virtual void SetBBox( Vector3 mins, Vector3 maxs) 
```
No Summary
```c#
virtual void StayOnGround( ) 
```
Try to keep a walking player on the ground when running down slopes etc
```c#
virtual void StepMove( ) 
```
No Summary
```c#
virtual void UpdateBBox( ) 
```
Update the size of the bbox. We should really trigger some shit if this changes.
```c#
virtual void UpdateGroundEntity( TraceResult tr) 
```
We have a new ground entity
```c#
virtual void WalkMove( ) 
```
No Summary
```c#
virtual void WaterMove( ) 
```
No Summary
```c#
override void FrameSimulate( ) 
```
OverridesBasePlayerController.FrameSimulateThis is called every frame on the client only
```c#
override BBox GetHull( ) 
```
OverridesBasePlayerController.GetHullThis is temporary, get the hull size for the player's collision
```c#
override void Simulate( ) 
```
OverridesPawnController.SimulateThis is what your logic should be going in
```c#
override TraceResult TraceBBox( Vector3 start, Vector3 end, float liftFeet = 0) 
```
OverridesBasePlayerController.TraceBBoxTraces the current bbox and returns the result.
liftFeet will move the start position up by this amount, while keeping the top of the bbox at the same
position. This is good when tracing down because you won't be tracing through the ceiling above.
