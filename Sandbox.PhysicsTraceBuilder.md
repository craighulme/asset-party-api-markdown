# PhysicsTraceBuilder

## Derives from ValueType

## Summary

Casts a PhysicsBody from its current position and rotation to desired end point.
## Methods

```c#
PhysicsTraceBuilder Body( PhysicsBody body, in Vector3 to) 
```
Casts a PhysicsBody from its current position and rotation to desired end point.
```c#
PhysicsTraceBuilder Body( PhysicsBody body, in Transform from, in Vector3 to) 
```
Casts a PhysicsBody from a position and rotation to desired end point.
```c#
PhysicsTraceBuilder Box( Vector3 extents, in Vector3 from, in Vector3 to) 
```
Casts a box from point A to point B.
```c#
PhysicsTraceBuilder Box( Vector3 extents, in Ray ray, in float distance) 
```
Casts a box from a given position and direction, up to a given distance.
```c#
PhysicsTraceBuilder Box( BBox bbox, in Vector3 from, in Vector3 to) 
```
Casts a box from point A to point B.
```c#
PhysicsTraceBuilder Box( BBox bbox, in Ray ray, in float distance) 
```
Casts a box from a given position and direction, up to a given distance.
```c#
PhysicsTraceBuilder Capsule( Capsule capsule) 
```
Casts a capsule
```c#
PhysicsTraceBuilder Capsule( Capsule capsule, in Vector3 from, in Vector3 to) 
```
Casts a capsule from point A to point B.
```c#
PhysicsTraceBuilder Capsule( Capsule capsule, in Ray ray, in float distance) 
```
Casts a capsule from a given position and direction, up to a given distance.
```c#
PhysicsTraceBuilder FromTo( in Vector3 from, in Vector3 to) 
```
Sets the start and end positions of the trace request
```c#
PhysicsTraceBuilder IncludeClientside( bool include = true) 
```
By default traces only hit entities and world that also exist on the server. This is the most common scenario as
if you hit client only entities during prediction you will get prediction errors.
You might however want to opt into including client entities in specific traces.
```c#
PhysicsTraceBuilder Radius( float radius) 
```
Makes this trace a sphere of given radius.
```c#
PhysicsTraceBuilder Ray( in Vector3 from, in Vector3 to) 
```
Casts a ray from point A to point B.
```c#
PhysicsTraceBuilder Ray( in Ray ray, in float distance) 
```
Casts a ray from a given position and direction, up to a given distance.
```c#
PhysicsTraceResult Run( ) 
```
Run the trace and return the result. The result will return the first hit.
```c#
PhysicsTraceBuilder Size( in BBox hull) 
```
Makes this trace an axis aligned box of given size. Extracts mins and maxs from the Bounding Box.
```c#
PhysicsTraceBuilder Size( in Vector3 size) 
```
Makes this trace an axis aligned box of given size. Calculates mins and maxs by assuming given size is (maxs-mins) and the center is in the middle.
```c#
PhysicsTraceBuilder Size( in Vector3 mins, in Vector3 maxs) 
```
Makes this trace an axis aligned box of given size.
```c#
PhysicsTraceBuilder Sphere( float radius, in Vector3 from, in Vector3 to) 
```
Casts a sphere from point A to point B.
```c#
PhysicsTraceBuilder Sphere( float radius, in Ray ray, in float distance) 
```
Casts a sphere from a given position and direction, up to a given distance.
```c#
PhysicsTraceBuilder Sweep( in PhysicsBody body, in Transform from, in Transform to) 
```
Sweeps eachPhysicsShapeof given PhysicsBody and returns the closest collision. Does not support Mesh PhysicsShapes.
Basically 'hull traces' but with physics shapes.
Same as tracing a body but allows rotation to change during the sweep.
```c#
PhysicsTraceBuilder Sweep( in PhysicsBody body, in Transform to) 
```
Creates a Trace.Sweep using thePhysicsBody's position as the starting position.
```c#
PhysicsTraceBuilder UseHitboxes( bool hit = true) 
```
Should we hit hitboxes
```c#
PhysicsTraceBuilder WithAllTags( string[] tags) 
```
Only return entities with all of these tags
```c#
PhysicsTraceBuilder WithAllTags( ITagSet tags) 
```
Only return entities with all of these tags
```c#
PhysicsTraceBuilder WithAnyTags( string[] tags) 
```
Only return entities with any of these tags
```c#
PhysicsTraceBuilder WithAnyTags( ITagSet tags) 
```
Only return entities with any of these tags
```c#
PhysicsTraceBuilder WithoutTags( string[] tags) 
```
Only return entities without any of these tags
```c#
PhysicsTraceBuilder WithoutTags( ITagSet tags) 
```
Only return entities without any of these tags
```c#
PhysicsTraceBuilder WithTag( string tag) 
```
Only return entities with this tag. Subsequent calls to this will add multiple requirements
and they'll all have to be met (ie, the entity will need all tags).
## Referencing Members

```c#
PhysicsTraceBuilder = PhysicsWorld.Trace { get; } 
```
