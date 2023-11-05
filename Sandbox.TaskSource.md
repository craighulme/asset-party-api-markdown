# TaskSource

## ```c#
Derives from ValueType
```

## Summary

Provides a way for us to cancel tasks after common async shit is executed.
## Properties

```c#
Task CompletedTask { get; } 
```
No Summary
```c#
bool IsValid { get; } 
```
Whether this object is valid or not.
## Methods

```c#
Task Delay( int ms) 
```
A task that does nothing for given amount of time in milliseconds.
```c#
Task DelayRealtime( int ms) 
```
No Summary
```c#
Task DelayRealtimeSeconds( float seconds) 
```
No Summary
```c#
Task DelaySeconds( float seconds) 
```
A task that does nothing for given amount of time in seconds.
```c#
void Expire( ) 
```
Marks this task source as invalid. All associated running tasks will be canceled ASAP.
```c#
Task<T> FromResult<T,>( T t) 
```
No Summary
```c#
Task MainThread( ) 
```
Continues on the main thread.
```c#
Task NextPhysicsFrame( ) 
```
Waits for the next physics frame.
```c#
Task RunInThreadAsync( Action action) 
```
No Summary
```c#
Task<T> RunInThreadAsync<T,>( Func<T> func) 
```
No Summary
```c#
Task RunInThreadAsync( Func<Task> task) 
```
No Summary
```c#
Task<T> RunInThreadAsync<T,>( Func<Task<T>> task) 
```
No Summary
```c#
void WaitAll( Task[] tasks) 
```
No Summary
```c#
void WaitAny( Task[] tasks) 
```
No Summary
```c#
Task WhenAll( Task[] tasks) 
```
No Summary
```c#
Task WhenAll( IEnumerable<Task> tasks) 
```
No Summary
```c#
Task<T[]> WhenAll<T,>( Task[] tasks) 
```
No Summary
```c#
Task<T[]> WhenAll<T,>( IEnumerable<Task<T>> tasks) 
```
No Summary
```c#
Task WhenAny( Task[] tasks) 
```
No Summary
```c#
Task WhenAny( IEnumerable<Task> tasks) 
```
No Summary
```c#
Task<Task<T>> WhenAny<T,>( Task[] tasks) 
```
No Summary
```c#
Task<Task<T>> WhenAny<T,>( IEnumerable<Task<T>> tasks) 
```
No Summary
```c#
Task WorkerThread( ) 
```
Continues on a worker thread.
```c#
Task Yield( ) 
```
No Summary
## Referencing Members

```c#
TaskSource = Entity.Task
```
```c#
TaskSource = Panel.Task
```
