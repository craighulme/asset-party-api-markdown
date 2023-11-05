# StreamUser

## 
```c#
Derives from ValueType
```

## Summary

Get followers "Who are we following"
## Properties

```c#
string BroadcasterType { get; } 
```
No Summary
```c#
DateTimeOffset CreatedAt { get; } 
```
No Summary
```c#
string Description { get; } 
```
No Summary
```c#
string DisplayName { get; } 
```
No Summary
```c#
string Email { get; } 
```
No Summary
```c#
Task<List<StreamUserFollow>> Followers { get; } 
```
Get followers "Who are we following"
```c#
Task<List<StreamUserFollow>> Following { get; } 
```
Get following "Who is following us"
```c#
string Id { get; } 
```
No Summary
```c#
string Login { get; } 
```
No Summary
```c#
string OfflineImageUrl { get; } 
```
No Summary
```c#
string ProfileImageUrl { get; } 
```
No Summary
```c#
string UserType { get; } 
```
No Summary
```c#
int ViewCount { get; } 
```
No Summary
## Methods

```c#
void Ban( string reason, int duration = 0) 
```
Ban user from your chat, the user will no longer be able to chat.
Optionally specify the duration, a duration of zero means perm ban
(Note: You have to be in your chat for this to work)
```c#
Task<StreamClip> CreateClip( bool hasDelay = false) 
```
Create a clip of our stream, if we're streaming
```c#
Task<StreamPoll> CreatePoll( string title, int duration, string[] choices) 
```
Start a poll on our channel with multiple choices, save the poll so you can end it later on
```c#
Task<StreamPrediction> CreatePrediction( string title, int duration, string firstOutcome, string secondOutcome) 
```
Create a prediction on our channel to bet with channel points
```c#
void Unban( ) 
```
Unban user from your chat, this allows them to chat again
(Note: You have to be in your chat for this to work)
## Referencing Members

```c#
static Task<StreamUser> = Streamer.GetUser( string ) 
```
