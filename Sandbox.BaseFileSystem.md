# BaseFileSystem

## ```c#
Derives from object
```

## Summary

Whether this object is valid or not.
## Properties

```c#
bool IsValid { get; } 
```
Whether this object is valid or not.
## Methods

```c#
void CreateDirectory( string folder) 
```
Create a directory - or a tree of directories.
Returns silently if the directory already exists.
```c#
BaseFileSystem CreateSubSystem( string path) 
```
Create a sub-filesystem at the specified path
```c#
void DeleteDirectory( string folder, bool recursive = false) 
```
Delete a folder and optionally all of its contents
```c#
void DeleteFile( string path) 
```
Delete a file
```c#
bool DirectoryExists( string path) 
```
Returns true if the directory exists on this filesystem
```c#
int DirectorySize( string path, bool recursive = false) 
```
Gets the size in bytes of all the files in a directory
```c#
bool FileExists( string path) 
```
Returns true if the file exists on this filesystem
```c#
long FileSize( string filepath) 
```
Returns file size of given file.
```c#
IEnumerable<string> FindDirectory( string folder, string pattern = "*", bool recursive = false) 
```
Get a list of directories
```c#
IEnumerable<string> FindFile( string folder, string pattern = "*", bool recursive = false) 
```
Get a list of files
```c#
Task<ulong> GetCRC( string filepath) 
```
Returns CRC64 of the file contents.
```c#
string GetFullPath( string path) 
```
Returns the full physical path to a file or folder on disk,
or null if it isn't on disk.
```c#
Stream OpenRead( string path, FileMode mode = 3) 
```
Open a file for read. Will throw an exception if it doesn't exist.
```c#
Stream OpenWrite( string path, FileMode mode = 2) 
```
Open a file for write. If the file exists we'll overwrite it (by default)
```c#
Span<byte> ReadAllBytes( string path) 
```
Read the contents of path and return it as a string
```c#
Task<byte[]> ReadAllBytesAsync( string path) 
```
Read the contents of path and return it as a string
```c#
string ReadAllText( string path) 
```
Read the contents of path and return it as a string.
Returns null if file not found.
```c#
Task<string> ReadAllTextAsync( string path) 
```
Read the contents of path and return it as a string
```c#
T ReadJson<T,>( string filename, T defaultValue = null) 
```
Read Json from a file using System.Text.Json.JsonSerializer. This will throw exceptions
if not valid json.
```c#
T ReadJsonOrDefault<T,>( string filename, T returnOnError = null) 
```
The same as ReadJson except will return a default value on missing/error.
```c#
void WriteAllText( string path, string contents) 
```
Write the contents to the path. The file will be over-written if the file exists
```c#
void WriteJson<T,>( string filename, T data) 
```
Convert object to json and write it to the specified file
