# NavMesh

## Is static
Derives from object

## Summary

Return if the nav mesh is loaded or not
## Properties

```c#
static bool IsLoaded { get; } 
```
Return if the nav mesh is loaded or not
## Methods

```c#
static Vector3[] BuildPath( Vector3 point, Vector3 end) 
```
Return an array of path positions
```c#
static bool BuildPath( Vector3 point, Vector3 end, List<Vector3> outPoints) 
```
Return an list of path positions
```c#
static NavAreaAttribute GetAreaAttribute( Vector3 point) 
```
Finds the closest nav area to a point and returns all the attributes associated with it as a bit flag.
```c#
static Vector3? GetClosestPoint( Vector3 point) 
```
Returns the closest point on the navmesh. Or null if not found.
```c#
static IEnumerable<NavArea> GetNavAreas( ) 
```
Get all the nav areas in the current loaded nav mesh
```c#
static Vector3? GetPointWithinRadius( Vector3 point, float minRadius, float maxRadius) 
```
Returns the closest point on the navmesh. Or null if not found.
```c#
static NavPathBuilder PathBuilder( Vector3 startPosition) 
```
Create a nav path builder with custom parameters
