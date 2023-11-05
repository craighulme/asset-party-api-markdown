# Friend

## Derives from ValueType

## Summary

The friend's Steam Id
## Constructors

```c#
Friend( long steamid) 
```
No Summary
## Properties

```c#
long Id { get; } 
```
The friend's Steam Id
```c#
bool IsAway { get; } 
```
Returns true if your friend is away
```c#
bool IsBusy { get; } 
```
Returns true if this friend is marked as busy
```c#
bool IsFriend { get; } 
```
Returns true if this user is your friend
```c#
bool IsMe { get; } 
```
Returns true if this friend is the local user
```c#
bool IsOnline { get; } 
```
Returns true if your friend is online
```c#
bool IsPlayingAGame { get; } 
```
Returns true if they're playing any game
```c#
bool IsPlayingThisGame { get; } 
```
Returns true if they're playing this game
```c#
bool IsSnoozing { get; } 
```
Returns true if this friend is marked as snoozing
```c#
string Name { get; } 
```
The friend's name
## Methods

```c#
static IEnumerable<Friend> GetAll( ) 
```
No Summary
```c#
string GetRichPresence( string key) 
```
Returns a string that was possibly set by rich presence
```c#
void OpenAddFriendOverlay( ) 
```
Opens the Steam overlay with a popup that allows the local Steam user to confirm whether to add this user to their Steam friends list.
```c#
void OpenInOverlay( ) 
```
Opens the Steam overlay web browser to their user profile.
## Referencing Members

```c#
Friend = VoiceEntry.Friend
```
```c#
abstract IEnumerable<Friend> = IGameMenu.Friends { get; } 
```
```c#
string = GameLobby.GetMemberData( Friend, string ) 
```
```c#
void GameLobby.InviteFriend( Friend ) 
```
```c#
static Task = PartyLobby.InviteFriend( Friend ) 
```
```c#
void GameLobby.Kick( Friend ) 
```
```c#
static void PartyLobby.Kick( Friend ) 
```
```c#
abstract IEnumerable<Friend> = ILobby.Members { get; } 
```
```c#
virtual IEnumerable<Friend> = GameLobby.Members { get; } 
```
```c#
virtual IEnumerable<Friend> = GlobalLobby.Members { get; } 
```
```c#
static IEnumerable<Friend> = PartyLobby.Members { get; } 
```
```c#
abstract Action<Friend, string> = ILobby.OnChatMessage { get; set; } 
```
```c#
virtual Action<Friend, string> = GameLobby.OnChatMessage { get; set; } 
```
```c#
virtual Action<Friend, string> = GlobalLobby.OnChatMessage { get; set; } 
```
```c#
abstract Action<Friend> = ILobby.OnMemberEnter { get; set; } 
```
```c#
virtual Action<Friend> = GameLobby.OnMemberEnter { get; set; } 
```
```c#
virtual Action<Friend> = GlobalLobby.OnMemberEnter { get; set; } 
```
```c#
abstract Action<Friend> = ILobby.OnMemberLeave { get; set; } 
```
```c#
virtual Action<Friend> = GameLobby.OnMemberLeave { get; set; } 
```
```c#
virtual Action<Friend> = GlobalLobby.OnMemberLeave { get; set; } 
```
```c#
abstract Friend = ILobby.Owner { get; set; } 
```
```c#
virtual Friend = GameLobby.Owner { get; set; } 
```
```c#
virtual Friend = GlobalLobby.Owner { get; set; } 
```
```c#
static Friend = PartyLobby.Owner { get; set; } 
```
```c#
abstract void ILobby.SendMessage( Friend, ByteStream, bool ) 
```
```c#
virtual void GameLobby.SendMessage( Friend, ByteStream, bool ) 
```
```c#
virtual void GlobalLobby.SendMessage( Friend, ByteStream, bool ) 
```
```c#
Friend = NetworkMessage.Source
```
