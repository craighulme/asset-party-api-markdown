# Trace

## ```c#
Derives from ValueType
```

## Summary

Casts a PhysicsBody from its current position and rotation to desired end point.
## Methods

```c#
static Trace Body( PhysicsBody body, in Vector3 to) 
```
Casts a PhysicsBody from its current position and rotation to desired end point.
```c#
static Trace Body( PhysicsBody body, in Transform from, in Vector3 to) 
```
Casts a PhysicsBody from a position and rotation to desired end point.
```c#
static Trace Box( Vector3 extents, in Vector3 from, in Vector3 to) 
```
Casts a box from point A to point B.
```c#
static Trace Box( Vector3 extents, in Ray ray, in float distance) 
```
Casts a box from a given position and direction, up to a given distance.
```c#
static Trace Box( BBox bbox, in Vector3 from, in Vector3 to) 
```
Casts a box from point A to point B.
```c#
static Trace Box( BBox bbox, in Ray ray, in float distance) 
```
Casts a box from a given position and direction, up to a given distance.
```c#
static Trace Capsule( Capsule capsule, in Vector3 from, in Vector3 to) 
```
Casts a capsule from point A to point B.
```c#
static Trace Capsule( Capsule capsule, in Ray ray, in float distance) 
```
Casts a capsule from a given position and direction, up to a given distance.
```c#
static Trace Ray( in Vector3 from, in Vector3 to) 
```
Casts a ray from point A to point B.
```c#
static Trace Ray( in Ray ray, in float distance) 
```
Casts a ray from a given position and direction, up to a given distance.
```c#
static Trace Sphere( float radius, in Vector3 from, in Vector3 to) 
```
Casts a sphere from point A to point B.
```c#
static Trace Sphere( float radius, in Ray ray, in float distance) 
```
Casts a sphere from a given position and direction, up to a given distance.
```c#
static Trace Sweep( in PhysicsBody body, in Transform from, in Transform to) 
```
Sweeps eachPhysicsShapeof given PhysicsBody and returns the closest collision. Does not support Mesh PhysicsShapes.
Basically 'hull traces' but with physics shapes.
Same as tracing a body but allows rotation to change during the sweep.
```c#
static Trace Sweep( in PhysicsBody body, in Transform to) 
```
Creates a Trace.Sweep using thePhysicsBody's position as the starting position.
```c#
static bool TestPoint( Vector3 point, string tag = "solid", float radius = 0.5) 
```
Returns true if point has an object
```c#
Trace DynamicOnly( ) 
```
This trace should only hit dynamic objects.
```c#
Trace EntitiesOnly( ) 
```
No Summary
```c#
Trace FromTo( in Vector3 from, in Vector3 to) 
```
Sets the start and end positions of the trace request
```c#
Trace Ignore( in IEntity ent, in bool hierarchy = true) 
```
Marks given entity to be ignored by the trace (the trace will go through it). Has a limit of 2 entities at this time.
```c#
Trace IncludeClientside( bool include = true) 
```
By default traces only hit entities and world that also exist on the server. This is the most common scenario as
if you hit client only entities during prediction you will get prediction errors.
You might however want to opt into including client entities in specific traces.
```c#
Trace Radius( float radius) 
```
Makes this trace a sphere of given radius.
```c#
TraceResult Run( ) 
```
Run the trace and return the result. The result will return the first hit.
If the trace didn't hit thenTraceResult.Hitwill be false.
```c#
TraceResult[] RunAll( ) 
```
Run the trace and return the results. This will return every entity hit in the
order that they were hit. It will only hit each entity once.
```c#
Trace Size( in BBox hull) 
```
Makes this trace an axis aligned box of given size. Extracts mins and maxs from the Bounding Box.
```c#
Trace Size( in Vector3 size) 
```
Makes this trace an axis aligned box of given size. Calculates mins and maxs by assuming given size is (maxs-mins) and the center is in the middle.
```c#
Trace Size( in Vector3 mins, in Vector3 maxs) 
```
Makes this trace an axis aligned box of given size.
```c#
Trace StaticOnly( ) 
```
This trace should only hit static objects.
```c#
Trace UseHitboxes( bool hit = true) 
```
Should we hit hitboxes
```c#
Trace WithAllTags( string[] tags) 
```
Only return entities with all of these tags
```c#
Trace WithAnyTags( string[] tags) 
```
Only return entities with any of these tags
```c#
Trace WithoutTags( string[] tags) 
```
Only return entities without any of these tags
```c#
Trace WithTag( string tag) 
```
Only return entities with this tag. Subsequent calls to this will add multiple requirements
and they'll all have to be met (ie, the entity will need all tags).
```c#
Trace WorldAndEntities( ) 
```
No Summary
```c#
Trace WorldOnly( ) 
```
No Summary
## Referencing Members

```c#
Trace = MoveHelper.Trace
```
