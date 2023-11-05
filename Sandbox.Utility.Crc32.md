# Crc32

## Is static
Derives from object

## Summary

Generate 32-bitCyclic Redundancy Check(CRC32) checksums.
## Methods

```c#
static uint FromBytes( IEnumerable<byte> byteStream) 
```
Generates a CRC32 checksum from a byte stream.
```c#
static Task<uint> FromStreamAsync( Stream stream) 
```
Generates a CRC32 checksum from a stream asynchronously.
```c#
static uint FromString( string str) 
```
Generates a CRC32 checksum from a string.
