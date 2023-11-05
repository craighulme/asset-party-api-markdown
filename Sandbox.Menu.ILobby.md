# ILobby

## 
```c#
Is interface
```

## Summary

A list of keyvalue datas stored on the lobby
## Properties

```c#
abstract ImmutableArray<string> Addons { get; set; } 
```
No Summary
```c#
abstract ImmutableDictionary<string, string> ConVars { get; set; } 
```
No Summary
```c#
abstract ImmutableDictionary<string, string> Data { get; } 
```
A list of keyvalue datas stored on the lobby
```c#
abstract string Description { get; set; } 
```
No Summary
```c#
abstract ulong Id { get; } 
```
No Summary
```c#
abstract bool IsMember { get; } 
```
No Summary
```c#
abstract string Map { get; set; } 
```
No Summary
```c#
abstract int MaxMembers { get; set; } 
```
No Summary
```c#
abstract int MemberCount { get; } 
```
No Summary
```c#
abstract IEnumerable<Friend> Members { get; } 
```
No Summary
```c#
abstract Action<Friend, string> OnChatMessage { get; set; } 
```
A new chat message has been recieved
```c#
abstract Action<Friend> OnMemberEnter { get; set; } 
```
A lobby member has entered
```c#
abstract Action<Friend> OnMemberLeave { get; set; } 
```
A lobby member has departed
```c#
abstract Friend Owner { get; set; } 
```
The owner of the lobby
```c#
abstract bool Public { get; set; } 
```
No Summary
```c#
abstract string SavedGame { get; set; } 
```
No Summary
```c#
abstract string State { get; set; } 
```
No Summary
```c#
abstract string Title { get; set; } 
```
No Summary
## Methods

```c#
abstract void BroadcastMessage( ByteStream msg, bool reliable = true) 
```
Broadcase a binary message to the lobby
```c#
abstract Task<bool> JoinAsync( ) 
```
No Summary
```c#
abstract Task LaunchGameAsync( ) 
```
If you're the host, will start the server. If you're a client, will try to join the game.
```c#
abstract void Leave( ) 
```
No Summary
```c#
abstract void OwnerMessage( ByteStream message, bool reliable = true) 
```
Send a message to the owner of the lobby
```c#
abstract void ReceiveMessages( NetworkMessageHandler action) 
```
Process incoming network messages
```c#
abstract void SendChat( string message) 
```
Broadcast a text message to the lobby. The id parameter defaults to 0
which is commonly used to signify a chat message.
```c#
abstract void SendMessage( Friend member, ByteStream message, bool reliable = true) 
```
Send a message to a member of the lobby
```c#
abstract void SetData( string key, string value) 
```
Change a value on the lobby
## Nested Types

