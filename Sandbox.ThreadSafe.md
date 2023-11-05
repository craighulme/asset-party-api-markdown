# ThreadSafe

## ```c#
Derives from object
```

## Summary

MainThread related functions.
## Properties

```c#
static int CurrentThreadId { get; } 
```
Return the current thread's Id (CurrentThread.ManagedThreadId)
```c#
static string CurrentThreadName { get; } 
```
Return the current thread's name (CurrentThread.Name)
```c#
static bool IsMainThread { get; } 
```
Returns true if we're executing under the main thread
## Methods

```c#
static void AssertIsMainThread( string memberName = "") 
```
Throws an exception if this is not called under the main thread
```c#
static void AssertIsNotMainThread( ) 
```
Throws an exception if this is the main thread
