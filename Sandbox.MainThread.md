# MainThread

## Is static
Derives from object

## Summary

Utility functions that revolve around the main thread
## Methods

```c#
static void Queue( Action method) 
```
When running in another thread you can queue a method to run in the main thread.
If you are on the main thread we will execute the method immediately and return.
