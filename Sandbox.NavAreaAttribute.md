# NavAreaAttribute

## 
```c#
Derives from Enum
```

## Summary

Avoid this area unless alternatives are too dangerous
## Fields

```c#
static NavAreaAttribute Avoid = 128
```
Avoid this area unless alternatives are too dangerous
```c#
static NavAreaAttribute Cliff = 32768
```
This nav area is adjacent to a drop of at least CliffHeight
```c#
static NavAreaAttribute Crouch = 1
```
Must crouch to use this node/area
```c#
static NavAreaAttribute Jump = 2
```
Must jump to traverse this area (only used during generation)
```c#
static NavAreaAttribute NoJump = 8
```
Inhibit discontinuity jumping
```c#
static NavAreaAttribute NoMerge = 8192
```
Don't merge this area with adjacent areas
```c#
static NavAreaAttribute ObstacleTop = 16384
```
This nav area is the climb point on the tip of an obstacle
```c#
static NavAreaAttribute Precise = 4
```
Do not adjust for obstacles, just move along area
```c#
static NavAreaAttribute Stairs = 4096
```
This area represents stairs, do not attempt to climb or jump them - just walk up
## Referencing Members

```c#
NavAreaAttribute = NavArea.Attributes { get; } 
```
```c#
static NavAreaAttribute = NavMesh.GetAreaAttribute( Vector3 ) 
```
