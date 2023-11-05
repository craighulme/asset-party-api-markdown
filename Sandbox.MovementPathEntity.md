# MovementPathEntity

## 
```c#
Derives from GenericPathEntity
```

## Summary

A movement path. Compiles each node as its own entity, allowing usage of inputs and outputs such as OnPassed.This entity can be used with entities like ent_path_platform.
## Constructors

```c#
MovementPathEntity( ) 
```
No Summary
## Properties

```c#
bool Looped { get; set; } 
```
Whether the path is looped or not.
## Methods

```c#
override void DrawPath( int segments, bool drawTangents = false) 
```
OverridesBasePathEntity<T>.DrawPath
