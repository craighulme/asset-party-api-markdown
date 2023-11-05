# SceneWorld

## ```c#
Implements IHandle
```

## Summary

A scene world that containsSandbox.SceneObjects. SeeUtility.CreateSceneWorld.You may also want aSandbox.SceneCamerato manually render the scene world.
## Constructors

```c#
SceneWorld( ) 
```
No Summary
## Fields

```c#
Color AmbientLightColor
```
Sets the ambient lighting color
```c#
Color ClearColor
```
No Summary
```c#
GradientFogController GradientFog
```
Controls gradient fog settings.
## Properties

```c#
IReadOnlyCollection<SceneObject> SceneObjects { get; } 
```
List of scene objects belonging to this scene world.
```c#
MeshTraceRequest Trace { get; } 
```
Trace against all scene objects in this scene world
## Methods

```c#
void Delete( ) 
```
Delete this scene world. You shouldn't access it anymore.
```c#
void DeletePendingObjects( ) 
```
Deleted objects are actually deleted at the end of each frame. Call this
to actually delete pending deletes right now instead of waiting.
