# GameManager

## Is abstract
Derives from BaseGameManager

## Summary

This is the main base game
## Constructors

```c#
GameManager( ) 
```
No Summary
## Properties

```c#
static GameManager Current { get; protected set; } 
```
ImplementsBaseGameManager.CurrentCurrently active game entity.
## Methods

```c#
virtual void DoPlayerDevCam( IClient client) 
```
The player wants to enable the devcam. Probably shouldn't allow this
unless you're in a sandbox mode or they're a dev.
```c#
virtual void MoveToSpawnpoint( Entity pawn) 
```
This entity is probably a pawn, and would like to be placed on a spawnpoint.
If you were making a team based game you'd want to choose the spawn based on team.
Or not even call this. Up to you. Added as a convenience.
```c#
virtual void OnKilled( Entity pawn) 
```
An entity has been killed. This is usually a pawn but anything can call it.
```c#
virtual void OnKilled( IClient client, Entity pawn) 
```
An entity, which is a pawn, and has a client, has been killed.
```c#
virtual void OnKilledMessage( long leftid, string left, long rightid, string right, string method) 
```
Called clientside from OnKilled on the server to add kill messages to the killfeed.
```c#
virtual void OnKilledMessage( To toTarget, long leftid, string left, long rightid, string right, string method) 
```
Called clientside from OnKilled on the server to add kill messages to the killfeed.
```c#
override void OnVoicePlayed( IClient cl) 
```
OverridesBaseGameManager.OnVoicePlayedSomeone is speaking via voice chat. This might be someone in your game,
or in your party, or in your lobby.
```c#
override void Shutdown( ) 
```
OverridesBaseGameManager.ShutdownCalled when the game is shutting down.
