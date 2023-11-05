# PhysicsBody

## Derives from object
Implements IHandle

## Summary

Represents a physics object. An entity can have multiple physics objects. SeePhysicsGroup.
A physics objects consists of one or morePhysicsShapes.
## Constructors

```c#
PhysicsBody( PhysicsWorld world) 
```
No Summary
## Properties

```c#
float AngularDamping { get; set; } 
```
Generic angular damping, i.e. how much the physics body will slow down on its own.
```c#
float AngularDrag { get; set; } 
```
Amount of air drag to be applied to angular movement/rotation. Default is 1.
This should take into account object's rotation and surface area in direction of rotation, unlikePhysicsBody.AngularDamping.
SeePhysicsWorld.AirDensityandPhysicsBody.DragEnabled.
```c#
Vector3 AngularVelocity { get; set; } 
```
Angular velocity of this body in world space.
```c#
bool AutoSleep { set; } 
```
Whether this body is allowed to automatically go into "sleep" after a certain amount of time of inactivity.PhysicsBody.Sleepingfor more info on the sleep mechanic.
```c#
PhysicsBodyType BodyType { get; set; } 
```
Movement type of physics body, either Static, Keyframed, Dynamic
Note: If this body is networked and dynamic, it will return Keyframed on the client
```c#
float Density { get; } 
```
Returns average of densities for all physics shapes of this body. This is based onPhysicsShape.SurfaceMaterialof each shape.
```c#
bool DragEnabled { get; set; } 
```
Whether air drag forces are enabled for this body.
SeePhysicsWorld.AirDensity,PhysicsBody.AngularDragandPhysicsBody.LinearDrag.
```c#
bool Enabled { get; set; } 
```
Whether this body is enabled or not. Disables collisions, physics simulation, touch events, trace queries, etc.
```c#
bool EnableSolidCollisions { get; set; } 
```
SetsPhysicsShape.EnableSolidCollisionson all shapes of this body.Returns true if ANY of the physics shapes have solid collisions enabled.
```c#
bool EnableTouch { get; set; } 
```
Enables Touch callbacks on allPhysicsShapesof this body.
Returns true if ANY of the physics shapes have touch events enabled.
```c#
bool EnableTouchPersists { get; set; } 
```
SetsPhysicsShape.EnableTouchPersistson all shapes of this body.Returns true if ANY of the physics shapes have persistent touch events enabled.
```c#
bool EnableTraceAndQueries { get; set; } 
```
SetsPhysicsShape.EnableTraceAndQuerieson all shapes of this body.Returns true if ANY of the physics shapes have traces and queries enabled.
```c#
object GameObject { get; set; } 
```
Per game usage data. Not used by the physics engine. Used to reconcile physics objects with game objects.
```c#
bool GravityEnabled { get; set; } 
```
Whether gravity is enabled for this body or not.
```c#
float GravityScale { get; set; } 
```
Scale the gravity relative toPhysicsWorld.Gravity. 2 is double the gravity, etc.
```c#
int GroupIndex { get; } 
```
Return the index of this body in its PhysicsGroup
```c#
string GroupName { get; } 
```
What is this body called in the group?
```c#
Vector3 Inertia { get; } 
```
The diagonal elements of the inertia tensor matrix.
```c#
Rotation InertiaRotation { get; } 
```
The orientation of the principal axes of inertia tensor matrix.
```c#
RealTimeSince LastWaterEffect { get; set; } 
```
Time since last water splash effect. Used internally.
```c#
float LinearDamping { get; set; } 
```
Generic linear damping, i.e. how much the physics body will slow down on its own.
```c#
float LinearDrag { get; set; } 
```
Amount of air drag to be applied to linear movement (i.e. not rotational movement). Default is 1.
This should take into account object's rotation and surface area in direction of movement, unlikePhysicsBody.LinearDamping.
SeePhysicsWorld.AirDensityandPhysicsBody.DragEnabled.
```c#
Vector3 LocalMassCenter { get; set; } 
```
Center of mass for this physics body relative to itsorigin.
```c#
float Mass { get; set; } 
```
Mass of this physics body.
```c#
Vector3 MassCenter { get; } 
```
Center of mass for this physics body in world space coordinates.
```c#
bool MotionEnabled { get; set; } 
```
Controls physics simulation on this body.
```c#
Action<PhysicsIntersectionEnd> OnIntersectionEnd { get; set; } 
```
No Summary
```c#
Action<PhysicsIntersection> OnIntersectionStart { get; set; } 
```
No Summary
```c#
Action<PhysicsIntersection> OnIntersectionUpdate { get; set; } 
```
No Summary
```c#
PhysicsBody Parent { get; set; } 
```
The physics body we are attached to, if any
```c#
PhysicsGroup PhysicsGroup { get; } 
```
The physics group we belong to.
```c#
Vector3 Position { get; set; } 
```
Position of this body in world coordinates.
```c#
Rotation Rotation { get; set; } 
```
Rotation of the physics body in world space.
```c#
float Scale { get; } 
```
Returns the scale of this object. (Most of the time inherited from owning entity's scale)
```c#
PhysicsBody SelfOrParent { get; } 
```
A convenience property, returnsParent, or if there is no parent, returns itself.
```c#
IEnumerable<PhysicsShape> Shapes { get; } 
```
All shapes that belong to this body.
```c#
bool Sleeping { get; set; } 
```
Physics bodies automatically go to sleep after a certain amount of time of inactivity to save on performance.
You can use this to wake the body up, or prematurely send it to sleep.
```c#
bool SpeculativeContactEnabled { get; set; } 
```
If enabled, this physics body will move slightly ahead each frame based on its velocities.
```c#
Surface Surface { get; set; } 
```
No Summary
```c#
string SurfaceMaterial { get; set; } 
```
SetsPhysicsShape.SurfaceMaterialon all childPhysicsShapes.
```c#
Transform Transform { get; set; } 
```
Transform of this physics body.
```c#
bool UseController { get; set; } 
```
If true we'll create a controller for this physics body. This is useful
for keyframed physics objects that need to push things. The controller will
sweep as the entity moves, rather than teleporting the object.. which works better
when pushing dynamic objects etc.
```c#
Vector3 Velocity { get; set; } 
```
Linear velocity of this body in world space.
```c#
PhysicsWorld World { get; } 
```
The physics world this body belongs to.
## Methods

```c#
PhysicsShape AddBoxShape( Vector3 position, Rotation rotation, Vector3 extent, bool rebuildMass = true) 
```
Add a box shape to this body.
```c#
PhysicsShape AddCapsuleShape( Vector3 center, Vector3 center2, float radius, bool rebuildMass = true) 
```
Add a capsule shape to this body.
```c#
PhysicsShape AddCloneShape( PhysicsShape shape) 
```
Clones given shape and adds it to this body.
```c#
PhysicsShape AddHullShape( Vector3 position, Rotation rotation, List<Vector3> points, bool rebuildMass = true) 
```
Add a convex hull shape to this body.
```c#
PhysicsShape AddHullShape( Vector3 position, Rotation rotation, Span<Vector3> points, bool rebuildMass = true) 
```
Add a convex hull shape to this body.
```c#
PhysicsShape AddMeshShape( List<Vector3> vertices, List<int> indices) 
```
Adds a mesh type shape to this physics body. Mesh shapes cannot be physically simulated!
```c#
PhysicsShape AddMeshShape( Span<Vector3> vertices, Span<int> indices) 
```
Adds a mesh type shape to this physics body. Mesh shapes cannot be physically simulated!
```c#
PhysicsShape AddShape( HullPart part, Transform transform, bool rebuildMass = true) 
```
Add a shape from a physics hull
```c#
PhysicsShape AddShape( MeshPart part, Transform transform, bool convertToHull, bool rebuildMass = true) 
```
Add a shape from a mesh hull
```c#
PhysicsShape AddSphereShape( Vector3 center, float radius, bool rebuildMass = true) 
```
Add a sphere shape to this body.
```c#
void ApplyAngularImpulse( Vector3 impulse) 
```
Applies instant angular impulse (i.e. a bullet impact) to this body.
For continuous force (i.e. a moving car), usePhysicsBody.ApplyTorque
```c#
void ApplyForce( Vector3 force) 
```
Applies force to this body at the center of mass.
This force will only be applied on the next physics frame and is scaled with physics timestep.
```c#
void ApplyForceAt( Vector3 position, Vector3 force) 
```
Applies force to this body at given position. This is akin to a bullet impact off center, and is capable of applying angular forces.
This force will only be applied on the next physics frame and is scaled with physics timestep.
```c#
void ApplyImpulse( Vector3 impulse) 
```
Applies instant linear impulse (i.e. a bullet impact) to this body at its center of mass.
For continuous force (i.e. a moving car), usePhysicsBody.ApplyForce
```c#
void ApplyImpulseAt( Vector3 position, Vector3 velocity) 
```
Applies instant linear impulse (i.e. a bullet impact) to this body at given position.
For continuous force (i.e. a moving car), usePhysicsBody.ApplyForceAt
```c#
void ApplyTorque( Vector3 force) 
```
Applies angular velocity to this body.
This force will only be applied on the next physics frame and is scaled with physics timestep.
```c#
bool CheckOverlap( PhysicsBody body) 
```
Checks if another body overlaps us, ignoring all collision rules
```c#
bool CheckOverlap( PhysicsBody body, Transform transform) 
```
Checks if another body overlaps us at a given transform, ignoring all collision rules
```c#
void ClearForces( ) 
```
Clear accumulated linear forces (PhysicsBody.ApplyForceandPhysicsBody.ApplyForceAt) during this physics frame that were not yet applied to the physics body.
```c#
void ClearShapes( ) 
```
Remove all physics shapes, but not the physics body itself.
```c#
void ClearTorque( ) 
```
Clear accumulated torque (angular force,PhysicsBody.ApplyTorque) during this physics frame that were not yet applied to the physics body.
```c#
Vector3 FindClosestPoint( Vector3 vec) 
```
Returns the closest point to the given one between all convex shapes of this body.
```c#
BBox GetBounds( ) 
```
Returns Axis-Aligned Bounding Box (AABB) of this physics body.
```c#
Vector3 GetVelocityAtPoint( Vector3 point) 
```
Returns the world space velocity of a point of the object. This is useful for objects rotating around their own axis/origin.
```c#
PhysicsPoint LocalPoint( Vector3 p) 
```
Convenience function that returns aPhysics.PhysicsPointfrom a position relative to this body.
```c#
PhysicsPoint MassCenterPoint( ) 
```
Returns aPhysics.PhysicsPointat the center of mass of this body.
```c#
void Move( Transform tx, float delta) 
```
Move to a new position. Unlike Transform, if you haveUseControllerenabled, this will sweep the shadow
to the new position, rather than teleporting there.
```c#
void RebuildMass( ) 
```
Meant to be only used ondynamicbodies, rebuilds mass from all shapes of this body based on their volume andphysics properties, for cases where they may have changed.
```c#
void Remove( ) 
```
Completely removes this physics body.
```c#
void SetMinSolverIterations( int minVelocityIterations, int minPositionIterations) 
```
No Summary
```c#
PhysicsPoint WorldPoint( Vector3 p) 
```
Convenience function that returns aPhysics.PhysicsPointfor this body from a world space position.
## Extensions

```c#
T GetEntity<T,>( ) 
```
Returns the entity this physics body belongs to.
```c#
Entity GetEntity( ) 
```
Returns the entity this physics body belongs to.
