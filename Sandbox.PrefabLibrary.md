# PrefabLibrary

## 
```c#
Derives from object
```

## Summary

Create an entity from an entity prefab. Throws exception if prefab isn't found.
## Methods

```c#
static void AssetReloaded( string path) 
```
No Summary
```c#
static T Spawn<T,>( string prefabName) 
```
Create an entity from an entity prefab. Throws exception if prefab isn't found.
```c#
static T Spawn<T,>( Prefab self) 
```
Create an entity from an entity prefab
```c#
static bool TrySpawn<T,>( string prefabName, out T createdEntity) 
```
Try to spawn an entity using the prefab name. Returns true on success.
