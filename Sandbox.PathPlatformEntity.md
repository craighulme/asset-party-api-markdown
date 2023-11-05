# PathPlatformEntity

## 
```c#
Derives from KeyframeEntity
```

## Summary

A platform that moves between nodes on a predefined path. See movement_path in the Path Tool.
## Constructors

```c#
PathPlatformEntity( ) 
```
No Summary
## Properties

```c#
OnEndAction EndAction { get; set; } 
```
What to do when reaching the end of the path when movement was initiated by the "StartMoving" input or "Starts Moving" flag. This also applies when moving backwards.
```c#
bool IsMoving { get; protected set; } 
```
Whether the platform is moving or not
```c#
bool IsMovingForwards { get; protected set; } 
```
The platform's move direction.
```c#
protected float Length { get; set; } 
```
This represents imaginary "distance to wheels" length from the center of the platform in either direction and is used to calculate correct angles when turning.Higher values will make turns smoother. This value should not exceed half of the platform's length in the direction of movement.
```c#
Angles MoveDir { get; set; } 
```
Specifies the direction to move in when the platform is used, or axis of rotation for rotating platforms.
```c#
string MovingSound { get; set; } 
```
Sound to play while platform is moving.
```c#
protected Output<int> OnAlreadyThere { get; set; } 
```
Fired when the platform is already at given node number, when using inputs to move it. Carries the current node number as parameter.
```c#
protected Output<int> OnMovementEnd { get; set; } 
```
Fired when the platform stops moving. Sends current point number as parameter.
```c#
protected Output OnMovementStart { get; set; } 
```
Fired when the platform starts to move.
```c#
EntityTarget PathEntity { get; set; } 
```
The path_generic entity that defines path nodes for this platform.
```c#
bool RotateAlongsidePath { get; set; } 
```
If set, the entity will automatically rotate to face the direction of movement. Moving backwards will NOT flip the rotation 180 degrees.
```c#
protected float Speed { get; set; } 
```
The speed to move/rotate with.
```c#
string StartMoveSound { get; set; } 
```
Sound to play when starting to move.
```c#
bool StartsMoving { get; set; } 
```
If set, will automatically start moving forwards from first node on spawn.
```c#
string StopMoveSound { get; set; } 
```
Sound to play when we stopped moving.
## Methods

```c#
GenericPathEntity GetPathEntity( ) 
```
Returns the actual path entity this platform is following, taking into account path changing.
```c#
void GoToNextPoint( ) 
```
Go to the next node on the path and stop there.
```c#
void GoToPoint( int targetNode) 
```
Go to specific node (Starting with 1) set by the parameter and stop there.
```c#
void GoToPrevPoint( ) 
```
Go to the previous node on the path and stop there.
```c#
void ReverseDirection( ) 
```
Reverse current movement direction, regardless whether we are currently moving or not.
```c#
void StartBackwards( ) 
```
Start moving backwards through our nodes until we reach start of the path.
```c#
void StartForward( ) 
```
Start moving forward through our nodes until we reach end of the path.
```c#
void StartMoving( ) 
```
Start moving through our nodes in whatever direction we were moving before until we reach either end of the path.
```c#
void StopMoving( ) 
```
Stop moving.
```c#
void WarpToPoint( int targetNode) 
```
Teleport to a given node (Starting with 1). Does not stop or start movement.
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
## Nested Types

