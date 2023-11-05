# NetWrite

## Derives from object
Implements IDisposable

## Summary

ImplementsIDisposable.Dispose
## Methods

```c#
static NetWrite StartRpc( int ident, Entity ent) 
```
No Summary
```c#
static NetWrite StartRpc2( int ident, BaseNetworkable networkable = null) 
```
No Summary
```c#
virtual void Dispose( ) 
```
ImplementsIDisposable.Dispose
```c#
void LengthAssert( long size) 
```
No Summary
```c#
void SendRpc( To? target, Entity from) 
```
No Summary
```c#
void SendRpc2( To? target, BaseNetworkable from = null) 
```
No Summary
```c#
void SendRpcToServer( Entity from) 
```
No Summary
```c#
void Write( byte[] buffer, int offset, int count) 
```
Write a raw sequence of bytes to the message.
```c#
void Write<T,>( T[] val) 
```
No Summary
```c#
void Write<T,>( Span<T> val) 
```
No Summary
```c#
void Write<T,>( T val) 
```
No Summary
```c#
void WriteObject( object obj) 
```
No Summary
```c#
void WriteUnmanagedArray<T,>( T[] arr) 
```
A dedicated method for writing an array of unmanaged types
```c#
void WriteUtf8( string str) 
```
No Summary
