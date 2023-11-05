# GameTask

## Is static
Derives from object

## Summary

A genericSandbox.TaskSource.
## Properties

```c#
static Task CompletedTask { get; } 
```
No Summary
## Methods

```c#
static Task Delay( int ms) 
```
A task that does nothing for given amount of time in milliseconds.
```c#
static Task DelayRealtime( int ms) 
```
No Summary
```c#
static Task DelayRealtimeSeconds( float seconds) 
```
No Summary
```c#
static Task DelaySeconds( float seconds) 
```
A task that does nothing for given amount of time in seconds.
```c#
static Task<T> FromResult<T,>( T t) 
```
No Summary
```c#
static SyncTask MainThread( ) 
```
Continues on the main thread.
```c#
static SyncTask NextPhysicsFrame( ) 
```
Waits for the next physics frame.
```c#
static Task RunInThreadAsync( Action action) 
```
No Summary
```c#
static Task<T> RunInThreadAsync<T,>( Func<T> func) 
```
No Summary
```c#
static Task RunInThreadAsync( Func<Task> task) 
```
No Summary
```c#
static Task<T> RunInThreadAsync<T,>( Func<Task<T>> task) 
```
No Summary
```c#
static void WaitAll( Task[] tasks) 
```
No Summary
```c#
static void WaitAny( Task[] tasks) 
```
No Summary
```c#
static Task WhenAll( Task[] tasks) 
```
No Summary
```c#
static Task WhenAll( IEnumerable<Task> tasks) 
```
No Summary
```c#
static Task<T[]> WhenAll<T,>( Task[] tasks) 
```
No Summary
```c#
static Task<T[]> WhenAll<T,>( IEnumerable<Task<T>> tasks) 
```
No Summary
```c#
static Task WhenAny( Task[] tasks) 
```
No Summary
```c#
static Task WhenAny( IEnumerable<Task> tasks) 
```
No Summary
```c#
static Task<Task<T>> WhenAny<T,>( Task[] tasks) 
```
No Summary
```c#
static Task<Task<T>> WhenAny<T,>( IEnumerable<Task<T>> tasks) 
```
No Summary
```c#
static SyncTask WorkerThread( ) 
```
Continues on a worker thread.
```c#
static Task Yield( ) 
```
No Summary
