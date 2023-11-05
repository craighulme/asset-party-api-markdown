# SyncTask

## ```c#
Implements INotifyCompletion
```

## Summary

ImplementsINotifyCompletion.OnCompleted
## Properties

```c#
bool IsCompleted { get; } 
```
No Summary
## Methods

```c#
virtual void OnCompleted( Action continuation) 
```
ImplementsINotifyCompletion.OnCompleted
```c#
SyncTask GetAwaiter( ) 
```
No Summary
```c#
void GetResult( ) 
```
No Summary
## Referencing Members

```c#
static SyncTask = GameTask.MainThread( ) 
```
```c#
static SyncTask = GameTask.NextPhysicsFrame( ) 
```
```c#
static SyncTask = GameTask.WorkerThread( ) 
```
