# IGameMenu

## Is interface

## Summary

Called from the loading screen.
This cancels whatever it's doing and returns to the main menu.
## Properties

```c#
abstract int FriendCount { get; } 
```
No Summary
```c#
abstract IEnumerable<Friend> Friends { get; } 
```
No Summary
```c#
abstract InputSettings InputSettings { get; } 
```
No Summary
```c#
abstract bool IsLoading { get; } 
```
No Summary
```c#
abstract ILobby[] Lobbies { get; } 
```
No Summary
```c#
abstract ILobby Lobby { get; } 
```
No Summary
```c#
abstract Package Package { get; } 
```
No Summary
```c#
abstract IEnumerable<SavedGame> SavedGames { get; } 
```
No Summary
## Methods

```c#
abstract void CancelLoading( ) 
```
Called from the loading screen.
This cancels whatever it's doing and returns to the main menu.
```c#
abstract bool ChangeServerMap( string ident) 
```
No Summary
```c#
abstract void Close( ) 
```
No Summary
```c#
abstract void ConnectToServer( ulong steamid) 
```
No Summary
```c#
abstract Task<ILobby> CreateLobbyAsync( int maxMembers, string cookieName = null, bool initGameSettings = false) 
```
No Summary
```c#
abstract Task CreateLobbyAsync( ) 
```
No Summary
```c#
abstract Task EnterServerAsync( ) 
```
No Summary
```c#
abstract string GetBind( string actionName, out bool isDefault, out bool isCommon) 
```
No Summary
```c#
abstract void HideMenu( ) 
```
No Summary
```c#
abstract void LeaveServer( string reason) 
```
No Summary
```c#
abstract Task<ILobby[]> QueryLobbiesAsync( string state = null, int withSlotsAvailable = 0) 
```
No Summary
```c#
abstract void ResetBinds( ) 
```
No Summary
```c#
abstract void SaveBinds( ) 
```
No Summary
```c#
abstract void SetBind( string actionName, string buttonName) 
```
No Summary
```c#
abstract Task StartServerAsync( int maxplayers, string hostname, string mapident) 
```
No Summary
```c#
abstract void TrapButtons( Action<string[]> callback) 
```
No Summary
