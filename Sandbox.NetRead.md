# NetRead

## ```c#
Derives from ValueType
```

## Summary

The amount of data (in bytes) remaining to be read
## Properties

```c#
int Remaining { get; } 
```
The amount of data (in bytes) remaining to be read
## Methods

```c#
static bool IsSupported( Type type) 
```
Get whether or not a type can be read by NetRead.
```c#
static bool IsSupported<T,>( Span<T> _) 
```
Get whether or not a value can be read by NetRead. This is a little
trick becauseGetType()does not work with Span.
```c#
static bool IsSupported( object value) 
```
Get whether or not a value can be read by NetRead.
```c#
void LengthAssert( int size) 
```
No Summary
```c#
int Read( byte[] buffer, int offset, int count) 
```
Read a raw sequence of bytes from the message, returning how many were read. May read less thancountif the end of the message is reached.
```c#
T Read<T,>( ) 
```
No Summary
```c#
T[] ReadArray<T,>( T[] val) 
```
No Summary
```c#
T[] ReadArrayClass<T,>( T[] val) 
```
No Summary
```c#
T ReadClass<T,>( T def = null) 
```
No Summary
```c#
Span<T> ReadData<T,>( Span<T> _) 
```
No Summary
```c#
T ReadData<T,>( T _) 
```
No Summary
```c#
object ReadObject( ) 
```
No Summary
```c#
string ReadString( ) 
```
No Summary
```c#
T[] ReadUnmanagedArray<T,>( T[] array) 
```
A dedicated method for arrays of unmanaged types that is faster to allow processing
of large arrays
```c#
T TryRead<T,>( ) 
```
Like read, but will return default if not enough size left
