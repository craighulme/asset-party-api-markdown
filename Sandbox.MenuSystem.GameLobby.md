# GameLobby

## Derives from object
Implements ILobby

## Summary

ImplementsILobby.AddonsProvides a list of addons (as their full idents) for this lobby
## Properties

```c#
virtual ImmutableArray<string> Addons { get; set; } 
```
ImplementsILobby.AddonsProvides a list of addons (as their full idents) for this lobby
```c#
virtual ImmutableDictionary<string, string> ConVars { get; set; } 
```
ImplementsILobby.ConVarsProvides a list of convars and their values for this lobby,
These will only be set properly if they match a Game Setting from the project's Project Settings page.
```c#
virtual string Description { get; set; } 
```
ImplementsILobby.DescriptionThe description of this lobby. What kind of game are they making?
```c#
virtual ulong Id { get; } 
```
ImplementsILobby.IdAccessor for the lobby ID
```c#
virtual bool IsMember { get; } 
```
ImplementsILobby.IsMemberAm I a member of this lobby? Checks the member list to find the local user.
```c#
virtual string Map { get; set; } 
```
ImplementsILobby.MapThe current map for this lobby
```c#
virtual int MaxMembers { get; set; } 
```
ImplementsILobby.MaxMembersMaximum number of people allowed in the lobby
```c#
virtual int MemberCount { get; } 
```
ImplementsILobby.MemberCountNumber of people in the lobby
```c#
virtual IEnumerable<Friend> Members { get; } 
```
ImplementsILobby.MembersAccessor to grab current lobby members
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
ImplementsILobby.OwnerGet the owner of the lobby. Only the owner of the lobby can change the owner.
```c#
virtual bool Public { get; set; } 
```
ImplementsILobby.Public
```c#
virtual string SavedGame { get; set; } 
```
ImplementsILobby.SavedGameThe name of the saved game to load.
```c#
virtual string State { get; set; } 
```
ImplementsILobby.StateThe current state of this lobby, ie "staging", "active"
```c#
virtual string Title { get; set; } 
```
ImplementsILobby.TitleThe title of this lobby. Think of this as the server name.
```c#
AccessMode Access { get; set; } 
```
No Summary
```c#
IEnumerable<KeyValuePair<string, string>> Data { get; } 
```
No Summary
```c#
string Game { get; set; } 
```
The game ident of this lobby.
```c#
ulong GameServer { get; set; } 
```
No Summary
```c#
bool IsJoinable { get; set; } 
```
No Summary
## Methods

```c#
static Task<GameLobby[]> GetList( string ident = null, string state = null) 
```
No Summary
```c#
static Task<GameLobby> TryJoinLobby( ulong lobbyId) 
```
Tries to join a lobby via its ID
```c#
virtual void BroadcastMessage( ByteStream message, bool reliable = true) 
```
ImplementsILobby.BroadcastMessageSend a message to everyone in the lobby
```c#
virtual Task<bool> JoinAsync( ) 
```
ImplementsILobby.JoinAsyncTry to join a lobby
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
ImplementsILobby.SendChatBroadcast a text message to the lobby.
```c#
virtual void SendMessage( Friend member, ByteStream message, bool reliable = true) 
```
ImplementsILobby.SendMessageSend a message to a member of the lobby
```c#
string GetData( string key) 
```
Get data associated with this lobby
```c#
string GetMemberData( Friend member, string key) 
```
Gets per-user metadata for someone in this lobby
```c#
void InviteFriend( Friend friend) 
```
Tries to send a lobby invite to a friend.
```c#
void InviteUsingOverlay( ) 
```
Opens platform specific overlay to select friends to invite to your lobby.
```c#
bool JoinGame( ) 
```
No Summary
```c#
void Kick( Friend friend) 
```
No Summary
```c#
void ReadyGameServer( ) 
```
Called by the lobby owner when the game server is ready.
```c#
bool RefreshData( ) 
```
You would never need to do this for a lobby you're part of.
```c#
bool SetData( string key, string value) 
```
ImplementsILobby.SetDataGet data associated with this lobby
```c#
void SetLocalMemberData( string key, string value) 
```
Sets per-user metadata (for the local user implicitly)
```c#
void StartGame( ) 
```
No Summary
```c#
Task ValidateMap( Package package) 
```
No Summary
## Nested Types

