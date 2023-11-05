# Streamer

## 
```c#
Derives from object
```

## Summary

Set the delay of your stream
## Properties

```c#
static int Delay { set; } 
```
Set the delay of your stream
```c#
static string Game { set; } 
```
Set the game you're playing by game id
```c#
static bool IsActive { get; } 
```
Are we connected to a service
```c#
static string Language { set; } 
```
Set the language of your stream
```c#
static StreamService Service { get; } 
```
The service type (ie "Twitch")
```c#
static string Title { set; } 
```
Set the title of your stream
```c#
static string UserId { get; } 
```
Your own user id
```c#
static string Username { get; } 
```
Your own username
```c#
static int ViewerCount { get; } 
```
Amount of concurrent viewer your stream has.
## Methods

```c#
static void BanUser( string username, string reason, int duration = 0) 
```
Ban user from your chat by username, the user will no longer be able to chat.
Optionally specify the duration, a duration of zero means perm ban
(Note: You have to be in your chat for this to work)
```c#
static void ClearChat( ) 
```
Clear your own chat
```c#
static Task<StreamUser> GetUser( string username = null) 
```
Get user information. If no username is specified, the user returned is ourself
```c#
static void SendMessage( string message) 
```
Send a message to chat, optionally specify channel you want to send the message, otherwise it is sent to your own chat
```c#
static void UnbanUser( string username) 
```
Unban user from your chat by username
(Note: You have to be in your chat for this to work)
