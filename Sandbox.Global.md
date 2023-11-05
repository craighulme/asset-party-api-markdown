# Global

## Is static
Derives from object

## Summary

Utility info for tools usage.
## Properties

```c#
static string BackendTitle { get; } 
```
Front facing identity for the backend
```c#
static string BackendUrl { get; } 
```
Url for the backend
```c#
static string GameIdent { get; } 
```
Identity of the gamemode the local client is currently playing.
```c#
static bool InGame { get; } 
```
Is the local client in game or not.
```c#
static bool IsApiConnected { get; } 
```
Are we connected to the API? (If not, offline mode. Requires Steam Servers to be online to connect..)
```c#
static bool IsContentMode { get; } 
```
Are we currently in Content Mode (no game selected)
```c#
static string MapName { get; } 
```
Name of the map the local client is on.
