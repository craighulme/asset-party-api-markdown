# PawnController

## ```c#
Derives from BaseNetworkable
```

## Summary

Allow the controller to tweak input. Empty by default.
## Constructors

```c#
PawnController( ) 
```
No Summary
## Properties

```c#
Vector3 BaseVelocity { get; set; } 
```
No Summary
```c#
IClient Client { get; protected set; } 
```
No Summary
```c#
Vector3 EyeLocalPosition { get; set; } 
```
No Summary
```c#
Rotation EyeRotation { get; set; } 
```
No Summary
```c#
Entity GroundEntity { get; set; } 
```
No Summary
```c#
Vector3 GroundNormal { get; set; } 
```
No Summary
```c#
Entity Pawn { get; protected set; } 
```
No Summary
```c#
Vector3 Position { get; set; } 
```
No Summary
```c#
Rotation Rotation { get; set; } 
```
No Summary
```c#
Vector3 Velocity { get; set; } 
```
No Summary
```c#
Vector3 WishVelocity { get; set; } 
```
No Summary
## Methods

```c#
virtual void BuildInput( ) 
```
Allow the controller to tweak input. Empty by default.
```c#
virtual void FrameSimulate( ) 
```
This is called every frame on the client only
```c#
virtual void OnEvent( string name) 
```
An event has been triggered - maybe handle it
```c#
virtual void RunEvents( PawnController additionalController) 
```
Call OnEvent for each event
```c#
virtual void Simulate( ) 
```
This is what your logic should be going in
```c#
void AddEvent( string eventName) 
```
Allows the controller to pass events to other systems
while staying abstracted.
For example, it could pass a "jump" event, which could then
be picked up by the playeranimator to trigger a jump animation,
and picked up by the player to play a jump sound.
```c#
void FrameSimulate( IClient client, Entity pawn) 
```
No Summary
```c#
bool HasEvent( string eventName) 
```
Returns true if we have this event
```c#
bool HasTag( string tagName) 
```

```c#
void SetTag( string tagName) 
```

```c#
void Simulate( IClient client, Entity pawn) 
```
No Summary
```c#
void UpdateFromController( PawnController controller) 
```
No Summary
```c#
void UpdateFromEntity( Entity entity) 
```
No Summary
## Inheriting Types

