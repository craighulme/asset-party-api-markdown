# ServerInformation

## Derives from ValueType

## Summary

Information about a server. This is sent from the server to the client
on client join to describe the server and tell the client what it needs
to download.
## Properties

```c#
string GameIdent { get; set; } 
```
The game's package ident
```c#
string GameTitle { get; set; } 
```
The title of the game. We send this too because the game might
not be on asset party, so the client wouldn't be able to get the real title.
```c#
string MapIdent { get; set; } 
```
The map's package ident
```c#
int MaxPlayers { get; set; } 
```
Get max players for the current server.
```c#
string[] RequiredContent { get; set; } 
```
If packages are required from asset party, they'll be listed here.
```c#
string ServerTitle { get; set; } 
```
The title of the server - changed with "hostname"
```c#
string SteamId { get; set; } 
```
The server's steamid
## Referencing Members

```c#
static ServerInformation = Game.Server { get; } 
```
