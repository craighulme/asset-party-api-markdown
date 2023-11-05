# MapLoader

## ```c#
Derives from object
```

## Summary

Create an object from a serialized object entry
## Constructors

```c#
MapLoader( SceneWorld world, PhysicsWorld physics) 
```
No Summary
## Fields

```c#
protected readonly List<SceneObject> SceneObjects
```
No Summary
## Properties

```c#
PhysicsWorld PhysicsWorld { get; } 
```
No Summary
```c#
SceneWorld World { get; } 
```
No Summary
## Methods

```c#
protected abstract void CreateObject( ObjectEntry kv) 
```
Create an object from a serialized object entry
## Inheriting Types

