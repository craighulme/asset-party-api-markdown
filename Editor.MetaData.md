# MetaData

## ```c#
Derives from object
```

## Summary

A class to CRUD json files. This should probably be a generic class since it seems
like we might want to do this with stuff other than meta files. But there's no need for
that right now, so lets leave it simple.
## Properties

```c#
string FilePath { get; } 
```
File path to the metadata file.
## Methods

```c#
T Get<T,>( string keyName, T defaultValue = null) 
```
No Summary
```c#
bool GetBool( string keyName, bool defaultValue = false) 
```
No Summary
```c#
JsonElement? GetElement( string keyName) 
```
No Summary
```c#
float GetFloat( string keyName, float defaultValue = 0) 
```
No Summary
```c#
int GetInt( string keyName, int defaultValue = 0) 
```
No Summary
```c#
string GetString( string keyName, string defaultValue = null) 
```
No Summary
```c#
void Set<T,>( string name, T value) 
```
Set a value in the metadata file. If the value is null, the key will be removed.
