# ByteStream

## Derives from ValueType

## Summary

A result of SpeedTest.MemoryAlloc - to make it easy to use this instead of AllocHGlobal
## Properties

```c#
int Length { get; } 
```
The total size of the data
```c#
int Position { get; set; } 
```
The current read or write position
```c#
int ReadRemaining { get; } 
```
No Summary
```c#
bool Writable { get; } 
```
No Summary
## Methods

```c#
static ByteStream Create( int size) 
```
Create a writable byte stream
```c#
static ByteStream CreateReader( ReadOnlySpan<byte> data) 
```
Create a writable byte stream
```c#
void Dispose( ) 
```
No Summary
```c#
void EnsureCanRead( int size) 
```
No Summary
```c#
void EnsureCanWrite( int size) 
```
No Summary
```c#
T Read<T,>( ) 
```
No Summary
```c#
string Read<T,>( string defaultValue = "") 
```
No Summary
```c#
T Read<T,>( T defaultValue = null, bool unused = false) 
```
No Summary
```c#
ReadOnlySpan<T> ReadArray<T,>( int maxElements = 1024) 
```
No Summary
```c#
object ReadObject( Type objectType) 
```
No Summary
```c#
byte[] ToArray( ) 
```
No Summary
```c#
bool TryRead<T,>( out T v) 
```
Try to read variable, return false if not enough data
```c#
void Write( ByteStream stream) 
```
No Summary
```c#
void Write( string str) 
```
Writing a string
```c#
void Write<T,>( T arr) 
```
Writing an unmanaged type
```c#
void Write<T,>( T data, bool unused = false) 
```
No Summary
```c#
void WriteArray<T,>( ReadOnlySpan<T> arr) 
```
Writing an array of unmanaged types
## Referencing Members

```c#
abstract void ILobby.BroadcastMessage( ByteStream, bool ) 
```
```c#
virtual void GameLobby.BroadcastMessage( ByteStream, bool ) 
```
```c#
virtual void GlobalLobby.BroadcastMessage( ByteStream, bool ) 
```
```c#
ByteStream = NetworkMessage.Data
```
```c#
abstract void ILobby.OwnerMessage( ByteStream, bool ) 
```
```c#
virtual void GameLobby.OwnerMessage( ByteStream, bool ) 
```
```c#
virtual void GlobalLobby.OwnerMessage( ByteStream, bool ) 
```
```c#
abstract void ILobby.SendMessage( Friend, ByteStream, bool ) 
```
```c#
virtual void GameLobby.SendMessage( Friend, ByteStream, bool ) 
```
```c#
virtual void GlobalLobby.SendMessage( Friend, ByteStream, bool ) 
```
