# IBasePathNode

## 
```c#
Is interface
```

## Summary

Used as both BasePathNode and BasePathNodeEntity so both can be used interchangeably
## Properties

```c#
abstract Vector3 WorldPosition { get; } 
```
Node's position in world space coordinates.
```c#
abstract Vector3 WorldTangentIn { get; } 
```
Node's incoming tangent in world space coordinates.
```c#
abstract Vector3 WorldTangentOut { get; } 
```
Node's outgoing tangent in world space coordinates.
