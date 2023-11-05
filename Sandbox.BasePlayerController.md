# BasePlayerController

## 
```c#
Derives from PawnController
```

## Summary

Any bbox traces we do will be offset by this amount.
todo: this needs to be predicted
## Constructors

```c#
protected BasePlayerController( ) 
```
No Summary
## Fields

```c#
Vector3 TraceOffset
```
Any bbox traces we do will be offset by this amount.
todo: this needs to be predicted
## Properties

```c#
static bool Debug { get; set; } 
```
No Summary
## Methods

```c#
virtual BBox GetHull( ) 
```
This is temporary, get the hull size for the player's collision
```c#
virtual TraceResult TraceBBox( Vector3 start, Vector3 end, Vector3 mins, Vector3 maxs, float liftFeet = 0) 
```
Traces the bbox and returns the trace result.
LiftFeet will move the start position up by this amount, while keeping the top of the bbox at the same
position. This is good when tracing down because you won't be tracing through the ceiling above.
```c#
virtual TraceResult TraceBBox( Vector3 start, Vector3 end, float liftFeet = 0) 
```
This calls TraceBBox with the right sized bbox. You should derive this in your controller if you
want to use the built in functions
```c#
override void FrameSimulate( ) 
```
OverridesPawnController.FrameSimulateThis is called every frame on the client only
## Inheriting Types

