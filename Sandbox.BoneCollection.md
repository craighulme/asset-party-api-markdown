# BoneCollection

## 
```c#
Derives from object
```

## Summary

A collection of bones. This could be from a model, or an entity
## Constructors

```c#
protected BoneCollection( ) 
```
No Summary
## Properties

```c#
abstract IReadOnlyList<Bone> AllBones { get; } 
```
List of all bones of our object.
```c#
abstract Bone Root { get; } 
```
Root bone of the model.
## Methods

```c#
Bone GetBone( string name) 
```
Retrieve a bone by name.
```c#
bool HasBone( string name) 
```
Whether the model or entity has a given bone by name.
## Nested Types

