# StreamPrediction

## 
```c#
Derives from ValueType
```

## Summary

Cancel this prediction
## Properties

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
DateTimeOffset CreatedAt { get; } 
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
DateTimeOffset LockedAt { get; } 
```
No Summary
```c#
Outcome[] Outcomes { get; } 
```
No Summary
```c#
int PredictionWindow { get; } 
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
```c#
string WinningOutcomeId { get; } 
```
No Summary
## Methods

```c#
Task<StreamPrediction> Cancel( ) 
```
Cancel this prediction
```c#
Task<StreamPrediction> Lock( ) 
```
Lock this prediction
```c#
Task<StreamPrediction> Resolve( ) 
```
Resolve this prediction and choose winning outcome to pay out channel points
## Nested Types

## Referencing Members

```c#
Task<StreamPrediction> = StreamUser.CreatePrediction( string, int, string, string ) 
```
