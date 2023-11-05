# StreamPoll

## 
```c#
Derives from ValueType
```

## Summary

End this poll, you can optionally archive the poll, otherwise just terminate it
## Properties

```c#
int BitsPerVote { get; } 
```
No Summary
```c#
bool BitsVotingEnabled { get; } 
```
No Summary
```c#
string BroadcasterId { get; } 
```
No Summary
```c#
string BroadcasterLogin { get; } 
```
No Summary
```c#
string BroadcasterName { get; } 
```
No Summary
```c#
int ChannelPointsPerVote { get; } 
```
No Summary
```c#
bool ChannelPointsVotingEnabled { get; } 
```
No Summary
```c#
Choice[] Choices { get; } 
```
No Summary
```c#
int Duration { get; } 
```
No Summary
```c#
DateTimeOffset EndedAt { get; } 
```
No Summary
```c#
string Id { get; } 
```
No Summary
```c#
DateTimeOffset StartedAt { get; } 
```
No Summary
```c#
string Status { get; } 
```
No Summary
```c#
string Title { get; } 
```
No Summary
## Methods

```c#
Task<StreamPoll> End( bool archive = true) 
```
End this poll, you can optionally archive the poll, otherwise just terminate it
## Nested Types

## Referencing Members

```c#
Task<StreamPoll> = StreamUser.CreatePoll( string, int, string[] ) 
```
