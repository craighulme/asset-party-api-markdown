# Map

## 
```c#
Derives from object
```

## Summary

The world physics objects
## Constructors

```c#
Map( string mapName, MapLoader loader) 
```
No Summary
## Properties

```c#
PhysicsGroup PhysicsGroup { get; } 
```
The world physics objects
```c#
SceneMap SceneMap { get; } 
```
The world physics objects
## Methods

```c#
static Task<Map> CreateAsync( string mapName, MapLoader loader, CancellationToken cancelToken = null) 
```
No Summary
```c#
void Delete( ) 
```
No Summary
