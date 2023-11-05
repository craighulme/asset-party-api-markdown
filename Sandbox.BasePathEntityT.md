# BasePathEntity<T>

## Derives from Entity

## Summary

A base entity that will appear in Hammer's Path Tool and automatically parse data from Hammer into a ready-to-use format in C#.
## Type Parameters

```c#
T is BasePathNode, 
```
No Summary
## Constructors

```c#
BasePathEntity( ) 
```
No Summary
## Properties

```c#
List<T> PathNodes { get; protected set; } 
```
A list of nodes this entity represents, as set up in Hammer.
```c#
protected string pathNodesJSON { get; set; } 
```
This is generated this automatically during map compile time
## Methods

```c#
static Entity FindPathEntity( string uniqueID) 
```
Internal, do not use. Used to link nodes to path entities. Finds a specific path entity and returns it.
```c#
virtual void DrawPath( int segments, bool drawTangents = false) 
```
Visualizes the path for debugging purposes
```c#
float GetCurveLength( IBasePathNode start, IBasePathNode end, int segments, bool reverse = false) 
```
Returns the approximate length of a curve between 2 nodes.
```c#
Vector3 GetPointBetweenNodes( IBasePathNode start, IBasePathNode end, float t, bool reverse = false) 
```
Returns a point in world space on the cubic beizer curve between 2 given nodes
```c#
override void ClientSpawn( ) 
```
OverridesEntity.ClientSpawnCalled when the entity spawns on client.
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
