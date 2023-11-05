# BaseGameManager

## ```c#
Derives from Entity
```

## Summary

This is the engine connection to the game entity.
You should derive your game fromSandbox.GameManagerrather than this.
## Constructors

```c#
BaseGameManager( ) 
```
No Summary
## Methods

```c#
virtual bool CanHearPlayerVoice( IClient source, IClient receiver) 
```
Can we hear the player's voice. If not we won't send the data to this client.
```c#
virtual void ClientDisconnect( IClient cl, NetworkDisconnectionReason reason) 
```
Client has disconnected from the server. Remove their entities etc.
```c#
virtual void ClientJoined( IClient cl) 
```
Client has joined the server. Create their puppets.
```c#
virtual void LoadSavedGame( SavedGame save) 
```
The game has been loaded from a previously saved game data. Override this to deserialize that data
and reconstruct your game from it.
```c#
virtual bool OnDragDropped( string text, Ray ray, string action) 
```
Something has been dragged and dropped on the game view. This is usually a file
from the asset browser. This is only called by the server host - so it's usually
safe to do stuff here without checking for cheats, depending on your game.
```c#
virtual bool OnEscapePressed( ) 
```
The escape button has been pressed. By default we send the escape key to the UI, and
if StopPropogation is set on the event, we swallow it. You can override this behaviour
in your game manager here to do whatever you want.
```c#
virtual void OnVoicePlayed( IClient cl) 
```
Someone is speaking via voice chat. This might be someone in your game,
or in your party, or in your lobby.
```c#
virtual void PostLevelLoaded( ) 
```
Called after the map has loaded.
```c#
virtual void RenderHud( ) 
```
Allows drawing the UI manually using Render.Draw2D etc
```c#
virtual bool ShouldConnect( long playerId) 
```
Called just after the player is authed. Can be used to reject connections before the client has joined.
The player's ClientEntity does not exist at this point.
Called by Sandbox.INetworkServer.ShouldConnect(System.Int64)
```c#
abstract void Shutdown( ) 
```
Called when the server is going away
```c#
override void BuildInput( ) 
```
OverridesEntity.BuildInputClientside only. Called every frame to process the input.
The results of this input are encoded into a user command and passed to the PlayerController both clientside and serverside.
This routine is mainly responsible for taking input from mouse/controller and building look angles and move direction.
```c#
override void FrameSimulate( IClient cl) 
```
OverridesEntity.FrameSimulateCalled each frame on the client only to simulate things that need to be updated every frame. An example
of this would be updating their local pawn's look rotation so it updates smoothly instead of at tick rate.
```c#
override void Simulate( IClient cl) 
```
OverridesEntity.SimulateCalled each tick.
Serverside: Called for each client every tick
Clientside: Called for each tick for local client. Can be called multiple times per tick.
## Inheriting Types

