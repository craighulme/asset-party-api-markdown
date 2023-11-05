# DataReceivedHandler

## Derives from MulticastDelegate

## Summary

Event handler which processes binary messages from the WebSocket service.
## Constructors

```c#
DataReceivedHandler( object object, IntPtr method) 
```
No Summary
## Methods

```c#
virtual IAsyncResult BeginInvoke( Span<byte> data, AsyncCallback callback, object object) 
```
No Summary
```c#
virtual void EndInvoke( IAsyncResult result) 
```
No Summary
```c#
virtual void Invoke( Span<byte> data) 
```
No Summary
