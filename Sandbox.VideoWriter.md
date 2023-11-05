# VideoWriter

## ```c#
Implements IDisposable
```

## Summary

Allows the creation of video content by encoding a sequence of frames.
## Properties

```c#
int Height { get; } 
```
No Summary
```c#
int Width { get; } 
```
No Summary
## Methods

```c#
virtual void Dispose( ) 
```
ImplementsIDisposable.DisposeDispose this recorder, the encoder will be flushed and video finalized.
```c#
bool AddFrame( ReadOnlySpan<byte> data, TimeSpan? timestamp = null) 
```
Add a frame of data to be encoded. Timestamp is in microseconds.
If a timestamp is not specified, it will use an incremented
frame count as the timestamp.
```c#
Task FinishAsync( ) 
```
Finish creating this video. The encoder will be flushed and video finalized.
## Nested Types

