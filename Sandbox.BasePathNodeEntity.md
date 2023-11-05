# BasePathNodeEntity

## ```c#
Implements IBasePathNode
```

## Summary

A basic node entity for theBasePathEntity.
These can be used as alternatives toBasePathNodedata structures with[Path]'s2nd argument.
## Constructors

```c#
BasePathNodeEntity( ) 
```
No Summary
## Properties

```c#
virtual Vector3 WorldPosition { get; } 
```
ImplementsIBasePathNode.WorldPositionNode's position in world space coordinates.
```c#
virtual Vector3 WorldTangentIn { get; } 
```
ImplementsIBasePathNode.WorldTangentInNode's incoming tangent in world space coordinates.
```c#
virtual Vector3 WorldTangentOut { get; } 
```
ImplementsIBasePathNode.WorldTangentOutNode's outgoing tangent in world space coordinates.
```c#
Entity PathEntity { get; protected set; } 
```
The Path entity this node belongs to.
```c#
Vector3 TangentIn { get; set; } 
```
Position of the incoming tangent relative to node's own position. Does NOT include node's rotation/scale.
```c#
Vector3 TangentOut { get; set; } 
```
Position of the outgoing tangent relative to node's own position. Does NOT include node's rotation/scale.
## Methods

```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
## Inheriting Types

