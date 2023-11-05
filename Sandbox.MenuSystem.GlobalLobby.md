# GlobalLobby

## 
```c#
Implements ILobby
```

## Summary

Simple global lobby
## Properties

```c#
static int Count { get; } 
```
No Summary
```c#
static GlobalLobby Instance { get; } 
```
No Summary
```c#
virtual ImmutableArray<string> Addons { get; set; } 
```
ImplementsILobby.Addons
```c#
virtual ImmutableDictionary<string, string> ConVars { get; set; } 
```
ImplementsILobby.ConVars
```c#
virtual ImmutableDictionary<string, string> Data { get; } 
```
ImplementsILobby.DataA list of keyvalue datas stored on the lobby
```c#
virtual string Description { get; set; } 
```
ImplementsILobby.Description
```c#
virtual ulong Id { get; } 
```
ImplementsILobby.Id
```c#
virtual bool IsMember { get; } 
```
ImplementsILobby.IsMember
```c#
virtual string Map { get; set; } 
```
ImplementsILobby.Map
```c#
virtual int MaxMembers { get; set; } 
```
ImplementsILobby.MaxMembers
```c#
virtual int MemberCount { get; } 
```
ImplementsILobby.MemberCount
```c#
virtual IEnumerable<Friend> Members { get; } 
```
ImplementsILobby.Members
```c#
virtual Action<Friend, string> OnChatMessage { get; set; } 
```
ImplementsILobby.OnChatMessageA new chat message has been recieved
```c#
virtual Action<Friend> OnMemberEnter { get; set; } 
```
ImplementsILobby.OnMemberEnterA lobby member has entered
```c#
virtual Action<Friend> OnMemberLeave { get; set; } 
```
ImplementsILobby.OnMemberLeaveA lobby member has departed
```c#
virtual Friend Owner { get; set; } 
```
ImplementsILobby.OwnerThe owner of the lobby
```c#
virtual bool Public { get; set; } 
```
ImplementsILobby.Public
```c#
virtual string SavedGame { get; set; } 
```
ImplementsILobby.SavedGame
```c#
virtual string State { get; set; } 
```
ImplementsILobby.State
```c#
virtual string Title { get; set; } 
```
ImplementsILobby.Title
## Methods

```c#
virtual void BroadcastMessage( ByteStream msg, bool reliable = true) 
```
ImplementsILobby.BroadcastMessageBroadcase a binary message to the lobby
```c#
virtual Task<bool> JoinAsync( ) 
```
ImplementsILobby.JoinAsync
```c#
virtual Task LaunchGameAsync( ) 
```
ImplementsILobby.LaunchGameAsyncIf you're the host, will start the server. If you're a client, will try to join the game.
```c#
virtual void Leave( ) 
```
ImplementsILobby.Leave
```c#
virtual void OwnerMessage( ByteStream message, bool reliable = true) 
```
ImplementsILobby.OwnerMessageSend a message to the owner of the lobby
```c#
virtual void ReceiveMessages( NetworkMessageHandler action) 
```
ImplementsILobby.ReceiveMessagesProcess incoming network messages
```c#
virtual void SendChat( string message) 
```
ImplementsILobby.SendChatBroadcast a text message to the lobby. The id parameter defaults to 0
which is commonly used to signify a chat message.
```c#
virtual void SendMessage( Friend member, ByteStream message, bool reliable = true) 
```
ImplementsILobby.SendMessageSend a message to a member of the lobby
```c#
virtual void SetData( string key, string value) 
```
ImplementsILobby.SetDataChange a value on the lobby
