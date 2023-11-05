# Context

## Derives from object

## Summary

Allows tracking states of button changes and input deltas in a custom period (such as a tick) rather
than in a per frame manner. This allows frame and tick to have legit data.
## Properties

```c#
string Name { get; } 
```
No Summary
## Methods

```c#
static Context Create( string name) 
```
No Summary
```c#
void Flip( ) 
```
Copy accumulated values. Flip previous actions to current actions etc.
```c#
IDisposable Push( ) 
```
Make this the current active context. You can optionally use the returned
IDisposable to restore back to the previous context when you're done.
