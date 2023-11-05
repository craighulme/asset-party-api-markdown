# PlatformEntity

## ```c#
Derives from KeyframeEntity
```

## Summary

A simple platform that moves between two locations and can be controlled through Entity IO.
## Constructors

```c#
PlatformEntity( ) 
```
No Summary
## Properties

```c#
float CurrentRotation { get; protected set; } 
```
Contains the current rotation of the platform in degrees.
```c#
bool IsMoving { get; protected set; } 
```
Whether the platform is moving or not
```c#
bool IsMovingForwards { get; protected set; } 
```
The platform's move direction.
```c#
bool LoopMovement { get; set; } 
```
If set, the platform will automatically go back upon reaching either end of the movement range.
```c#
Angles MoveDir { get; set; } 
```
Specifies the direction to move in when the platform is used, or axis of rotation for rotating platforms.
```c#
bool MoveDirIsLocal { get; set; } 
```
If checked, the movement direction angle is in local space and should be rotated by the entity's angles after spawning.
```c#
PlatformMoveType MoveDirType { get; set; } 
```
Movement type of the platform.Moving: Moving linearly and reversing direction at final position if Looping is enabled.Rotating: Rotating and reversing direction at final rotation if Looping is enabled.Rotating Continuous: Rotating continuously past Move Distance. OnReached outputs are fired every Move Distance degrees.
```c#
float MoveDistance { get; set; } 
```
How much to move in the move direction, or rotate around the axis for rotating move type.
```c#
string MovingSound { get; set; } 
```
Sound to play while platform is moving.
```c#
protected Output OnReachedEnd { get; set; } 
```
Fired when the platform reaches its end location (startPos + dir * distance)
```c#
protected Output OnReachedStart { get; set; } 
```
Fired when the platform reaches its beginning location
```c#
float Speed { get; protected set; } 
```
The speed to move/rotate with.
```c#
string StartMoveSound { get; set; } 
```
Sound to play when starting to move
```c#
float StartPosition { get; set; } 
```
At what percentage between start and end positions should the platform spawn in
```c#
bool StartsMoving { get; set; } 
```
If set, the platform will start moving on spawn.
```c#
string StopMoveSound { get; set; } 
```
Sound to play when we stopped moving
```c#
float TimeToHold { get; set; } 
```
If set to above 0 andLoop Movementis enabled, the amount of time to wait before automatically toggling direction.
## Methods

```c#
void ReverseMoving( ) 
```
Reverse current move direction. Will NOT start moving if stopped
```c#
void SetSpeed( float speed) 
```
Sets the move speed
```c#
void StartMoving( ) 
```
Start moving in platform's current move direction
```c#
void StartMovingBackwards( ) 
```
Set the move direction to backwards and start moving
```c#
void StartMovingForward( ) 
```
Set the move direction to forwards and start moving
```c#
void StopMoving( ) 
```
Stop moving, preserving move direction
```c#
void ToggleMoving( ) 
```
Toggle moving, preserving move direction
```c#
protected override void OnDestroy( ) 
```
OverridesEntity.OnDestroyCalled when the entity was destroyed. This is not the same as the class destructor.
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
## Nested Types

