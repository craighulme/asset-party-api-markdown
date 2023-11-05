# Crc64

## 
```c#
Derives from object
```

## Summary

Generate 64-bitCyclic Redundancy Check(CRC64) checksums.
## Methods

```c#
static ulong FromBytes( byte[] stream) 
```
Generates a CRC64 checksum from a byte array.
```c#
static ulong FromStream( Stream stream) 
```
Generates a CRC64 checksum from a stream.
```c#
static Task<ulong> FromStreamAsync( Stream stream) 
```
Generates a CRC64 checksum from a stream asynchronously.
```c#
static ulong FromString( string str) 
```
Generates a CRC64 checksum from a string.
