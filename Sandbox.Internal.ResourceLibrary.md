# ResourceLibrary

## Derives from object

## Summary

Keeps a library of all availableSandbox.GameResource.
## Methods

```c#
T Get<T,>( int identifier) 
```
Get a cached resource by its hash.
```c#
T Get<T,>( string filepath) 
```
Get a cached resource by its file path.
```c#
IEnumerable<T> GetAll<T,>( ) 
```
Get all cached resources of given type.
```c#
bool TryGet<T,>( string filepath, out T resource) 
```
Try to get a cached resource by its file path.
