# NavPathBuilder

## Derives from ValueType

## Summary

Add an extra stop along the path
## Constructors

```c#
NavPathBuilder( Vector3 startPosition) 
```
No Summary
## Methods

```c#
static NavPathBuilder Create( Vector3 startPosition) 
```
No Summary
```c#
NavPathBuilder AddStop( Vector3 position) 
```
Add an extra stop along the path
```c#
NavPathBuilder AddStop( Entity targetEntity) 
```
Add an extra stop along the path
```c#
NavPath Build( Entity targetEntity) 
```
Compute the nav path and return it
```c#
NavPath Build( Vector3 endPosition) 
```
Compute the nav path and return it
```c#
NavPathBuilder WithAgentHull( NavAgentHull hull) 
```
Specify which agent hull we should use for path finding
```c#
NavPathBuilder WithDropDistanceCostScale( float scale) 
```
Scales the drop distance of the path by some number. The larger this is the more unlikely the NPC
is to drop down and the more likely the NPC will take an alternate path
```c#
NavPathBuilder WithDuckHeight( float duckHeight) 
```
Characters duck hull height
```c#
NavPathBuilder WithMaxClimbDistance( float distance) 
```
Maximum climb up distance
```c#
NavPathBuilder WithMaxDetourDistance( float distance) 
```
Set how much we can detour from our path
```c#
NavPathBuilder WithMaxDistance( float distance) 
```
Set the maximum desired path length
```c#
NavPathBuilder WithMaxDropDistance( float distance) 
```
Maximum drop down distance
```c#
NavPathBuilder WithNoOptimization( ) 
```
Disable optimization and cleaning up nav path
```c#
NavPathBuilder WithPartialPaths( ) 
```
Are we allowed to generate an incomplete path?
```c#
NavPathBuilder WithPathSpeed( float speed) 
```
Requested speed along the path
```c#
NavPathBuilder WithSharpStartAngle( float angle) 
```
If positive, then path starts above this angle threshold (relative to NPC's current velocity) will start with a sharp turn instead of a smooth path.
```c#
NavPathBuilder WithSpringConstant( float k) 
```
Spring const toward lookahead point (and velocity) on path
```c#
NavPathBuilder WithSpringTensionMax( float tension) 
```
Maximum velocity delta than can be requested of the spring follower
```c#
NavPathBuilder WithStartAcceleration( Vector3 acceleration) 
```
Acceleration at start of path on the X/Y plane
```c#
NavPathBuilder WithStartVelocity( Vector3 velocity) 
```
Velocity at start of path on the X/Y plane
```c#
NavPathBuilder WithStepHeight( float stepHeight) 
```
The step size of the character
## Referencing Members

```c#
static NavPathBuilder = NavMesh.PathBuilder( Vector3 ) 
```
