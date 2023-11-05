# SceneMap

## ```c#
Implements IValid
```

## Summary

Map geometry that can be rendered within aSandbox.SceneWorld.
## Constructors

```c#
SceneMap( SceneWorld sceneWorld, string map) 
```
Create a scene map within a scene world.
## Properties

```c#
virtual bool IsValid { get; } 
```
ImplementsIValid.IsValidIs the map valid.
```c#
BBox Bounds { get; } 
```
Bounds of the map.
```c#
string MapName { get; } 
```
No Summary
```c#
SceneWorld World { get; } 
```
The scene world this map belongs to.
## Methods

```c#
static Task<SceneMap> CreateAsync( SceneWorld sceneWorld, string map, CancellationToken cancelToken = null) 
```
Create scene map asynchronously for when large maps take time to load.
```c#
void Delete( ) 
```
Delete this scene map. You shouldn't access it anymore.
