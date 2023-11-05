# NavigationMesh

## 
```c#
Implements IDisposable, IWeakInteropHandle
```

## Summary

Navigation Mesh - allowing AI to navigate a world
## Constructors

```c#
NavigationMesh( ) 
```
No Summary
## Properties

```c#
Dictionary<uint, Node> Nodes { get; } 
```
No Summary
## Methods

```c#
virtual void Dispose( ) 
```
ImplementsIDisposable.Dispose
```c#
void Generate( PhysicsWorld world) 
```
No Summary
```c#
void Load( byte[] data) 
```
Load the navmesh from a serialized value
```c#
void Load( string filename) 
```
Load the navmesh from a file (can be inside a vpk)
```c#
byte[] Save( ) 
```
Get the serialized byte value of this NavMesh
## Nested Types

