# PartyLobby

## Is static
Derives from object

## Summary

Basic Steam Lobby with members, chat and rich presence.
## Properties

```c#
static int MemberCount { get; } 
```
Prefer to Members.Count()
```c#
static IEnumerable<Friend> Members { get; } 
```
Party members
```c#
static Friend Owner { get; set; } 
```
Party owner
## Methods

```c#
static Task InviteFriend( Friend friend) 
```
Tries to send a lobby invite to a friend.
```c#
static Task<bool> Join( ulong id) 
```
No Summary
```c#
static void Kick( Friend friend) 
```
No Summary
```c#
static void Leave( ) 
```
No Summary
```c#
static Task SendChat( string message) 
```
Sends a chat message to the party
