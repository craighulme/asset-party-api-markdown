# MoveHelper

## 
```c#
Derives from ValueType
```

## Summary

This is the HL2 style movement. If moving fromMoveHelper.PositionusingMoveHelper.Velocityresults
in a collision, velocity will be changed to slide across the surface where
appropriate. Position will be updated to the optimal position.This is coded to be simple on purpose. It's enough to get your started. Once you
reach the point where it's lacking you should copy and paste it into your project
and specialize to your needs.Give it a position and velocity, set the Trace up how you want to
use it, then you're good to go.
## Constructors

```c#
MoveHelper( Vector3 position, Vector3 velocity, string[] solidTags) 
```
Create the movehelper and initialize it with the default settings.
You can change Trace and MaxStandableAngle after creation.
```c#
MoveHelper( Vector3 position, Vector3 velocity) 
```
Create the movehelper and initialize it with the default settings.
You can change Trace and MaxStandableAngle after creation.
## Fields

```c#
float GroundBounce
```
No Summary
```c#
bool HitWall
```
No Summary
```c#
float MaxStandableAngle
```
No Summary
```c#
Vector3 Position
```
No Summary
```c#
Trace Trace
```
No Summary
```c#
Vector3 Velocity
```
No Summary
```c#
float WallBounce
```
No Summary
## Methods

```c#
void ApplyFriction( float frictionAmount, float delta) 
```
Apply an amount of friction to the velocity
```c#
bool IsFloor( TraceResult tr) 
```
Return true if this is the trace is a floor. Checks hit and normal angle.
```c#
TraceResult TraceDirection( Vector3 down) 
```
Trace this from its current Position to a delta
```c#
TraceResult TraceFromTo( Vector3 start, Vector3 end) 
```
Trace this from one position to another
```c#
TraceResult TraceMove( Vector3 delta) 
```
Move our position by this delta using trace. If we hit something we'll stop,
we won't slide across it nicely like TryMove does.
```c#
float TryMove( float timestep) 
```
Try to move to the position. Will return the fraction of the desired velocity that we traveled.
Position and Velocity will be what we recommend using.
```c#
float TryMoveWithStep( float timeDelta, float stepsize) 
```
Like TryMove but will also try to step up if it hits a wall
```c#
bool TryUnstuck( ) 
```
Test whether we're stuck, and if we are then unstuck us
