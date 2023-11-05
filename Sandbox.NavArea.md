# NavArea

## 
```c#
Derives from object
```

## Summary

Amount of adjacent nav areas
## Properties

```c#
int AdjacentCount { get; } 
```
Amount of adjacent nav areas
```c#
NavAreaAttribute Attributes { get; } 
```
Attributes of the nav area
```c#
Vector3 Center { get; } 
```
Center of the nav area
```c#
uint ID { get; } 
```
Unique ID of the nav area
```c#
Vector3 Normal { get; } 
```
Normal of the nav area
```c#
bool Valid { get; } 
```
Is this area valid?
## Methods

```c#
static NavArea GetClosestNav( Vector3 Position, NavAgentHull HullIndex, GetNavAreaFlags GetNavFlags, ref Vector3 pNearestPosOut, float MaxDist = 10000, float BeneathLimit = 80, float AboveLimit = 18, float SideLimit = 16) 
```
Get the closest nav area from a given point
```c#
static NavArea GetClosestNav( Vector3 Position, NavAgentHull HullIndex = 0, GetNavAreaFlags GetNavFlags = 0, float MaxDist = 10000, float BeneathLimit = 80, float AboveLimit = 18, float SideLimit = 16) 
```
Get the closest nav area from a given point
```c#
Vector3 FindRandomConnectedPoint( Vector3 StartPosition, NavAgentHull HullIndex, float MaxDistance, float MinDistance = 0) 
```
Return a random point which is reachable from the current nav mesh
```c#
Vector3 FindRandomSpot( ) 
```
Return a random point on the nav area
```c#
IEnumerable<NavArea> GetAdjancent( NavDirection direction) 
```
Get all adjacent nav areas from the current nav area in a specific direction
```c#
NavArea GetRandomAdjacent( ) 
```
Return a random adjacent nav area
