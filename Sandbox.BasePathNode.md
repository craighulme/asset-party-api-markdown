# BasePathNode

## 
```c#
Implements IBasePathNode
```

## Summary

A basic node description for theBasePathEntity.
Please note thatBasePathNodesare NOT actual entities, therefore cannot support inputs and outputs. SeeBasePathNodeEntity.
## Constructors

```c#
BasePathNode( ) 
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
Entity Entity { get; set; } 
```
The entity associated with this path node, if they were set to spawn via[Path]This will be set as soon as the node entity spawns, which will be after Path entity's Spawn() function.
```c#
string HammerUniqueId { get; set; } 
```
Used to set the Entity property. Couldn't find a way to hide it. Do not use.
```c#
Entity PathEntity { get; } 
```
The path entity this node is associated with.
```c#
Vector3 Position { get; set; } 
```
Position of the node relative to the path entity.
```c#
Vector3 TangentIn { get; set; } 
```
Position of the incoming tangent relative to the node's position. Includes rotation/scale of the node.
```c#
Vector3 TangentOut { get; set; } 
```
Position of the outgoing tangent relative to the node's position. Includes rotation/scale of the node.
