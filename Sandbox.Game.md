# Game

## Is static
Derives from object

## Summary

Steam AppId of S&box.
## Properties

```c#
static ulong AppId { get; } 
```
Steam AppId of S&box.
```c#
static IReadOnlyCollection<IClient> Clients { get; } 
```
Returns a list of all clients on the server.
```c#
static Color Color { get; } 
```
Color or the current realm. Will either be Cyan for server, Orange for client or Green for menu.
```c#
static SavedGame CurrentSavedGame { get; } 
```
The currently loaded Saved Game.
```c#
static SceneWorld DebugSceneWorld { get; } 
```
No Summary
```c#
static bool InGame { get; } 
```
Return true if we're in a game (ie, not in the main menu)
```c#
static bool IsClient { get; } 
```
Returns true only when current code is running on the client.
```c#
static bool IsClosing { get; } 
```
Set to true when the game is closing
```c#
static bool IsDedicatedServer { get; } 
```
Whether this is a dedicated server.
```c#
static bool IsEditor { get; } 
```
Returns true if the game is running with the editor enabled
```c#
static bool IsListenServer { get; } 
```
Whether this server is a listen server, i.e. a server started on the game client.
```c#
static bool IsMainMenuVisible { get; } 
```
Returns true if the main menu is visible. Note that this will work serverside too but will only
return the state of the host.
```c#
static bool IsPlayingDemo { get; } 
```
Whether the engine is currently playing a demo - a recording of a game.
```c#
static bool IsRecordingVideo { get; } 
```
True if we're currently recording a video (using the video command, or F6)
```c#
static bool IsRunningInVR { get; } 
```
Return true if we're running in VR. Will always be false serverside.
```c#
static bool IsRunningOnHandheld { get; } 
```
Return true if we're running on a handheld device (the deck). Will always be false serverside.
```c#
static bool IsServer { get; } 
```
Returns true only when current code is running on the server.
```c#
static bool IsServerHost { get; } 
```
If we're hosting the server will return true. Will always return true serverside.
```c#
static bool IsToolsEnabled { get; } 
```
No Summary
```c#
static bool IsToolsMode { get; } 
```
No Summary
```c#
static IClient LocalClient { get; } 
```
The local client. This is you if you're connecting to the server.
```c#
static Entity LocalPawn { get; } 
```
The local client's pawn. This is probably a player, or a vehicle, or a melon.
```c#
static IGameMenu Menu { get; } 
```
The current game menu screen
```c#
static PhysicsWorld PhysicsWorld { get; } 
```
The current game's scene world
```c#
static Random Random { get; } 
```
A shared random that is automatically seeded on tick
```c#
static RootPanel RootPanel { get; set; } 
```
This might point to the root panel of the in game HUD. If the game sets it to it.
```c#
static SceneWorld SceneWorld { get; } 
```
The current game's scene world
```c#
static ServerInformation Server { get; } 
```
Information about the server we're currently connected to.
```c#
static ulong ServerSteamId { get; } 
```
64-bit SteamID of the server, used to connect to it.
```c#
static long SteamId { get; } 
```
Your SteamId
```c#
static float TickInterval { get; } 
```
1 / TickRate
```c#
static int TickRate { get; set; } 
```
Amount of ticks to perform per second. Higher is smoother and more accurate but uses more
power. Lower can be laggy and weird things can happen. Default is 50.
```c#
static float TimeScale { get; set; } 
```
Scale the time, globally
```c#
static string UserName { get; } 
```
Your Steam Name
```c#
static WorldEntity WorldEntity { get; } 
```
The main world entity
## Methods

```c#
static void AssertClient( string memberName = "") 
```
Throws an exception when called from server or menu.
```c#
static void AssertClientOrMenu( string memberName = "") 
```
Throws an exception when called from server.
```c#
static void AssertMenu( string memberName = "") 
```
Throws an exception when called from client or server.
```c#
static void AssertNotServer( string memberName = "") 
```
Throws an exception when called from client or menu.
```c#
static void AssertServer( string memberName = "") 
```
Throws an exception when called from client or menu.
```c#
static void ChangeLevel( string mapName) 
```
Change the currently loaded level. This is serverside only.
```c#
static WebSurface CreateWebSurface( ) 
```
Create a limited web surface
```c#
static void Disconnect( ) 
```
Disconnect from the current game session
```c#
static void ResetMap( Entity[] keepEntities) 
```
Cleans up the map to its original state. Pass in any entities you want to keep around, which
will likely be anything you have spawned at runtime. We automatically skip over Clients, World
and Gamemode - so don't worry about passing them in. For example you might want to pass in your HUD entity
if you have one.You can also stop entities getting reset by giving them the"ignorereset"tag.
```c#
static void Save( SavedGame save) 
```
Create a saved game. Previously saved games can be loaded during game creation.
```c#
static void SetRandomSeed( int seed) 
```
Set the seed for Game.Random
## Nested Types

