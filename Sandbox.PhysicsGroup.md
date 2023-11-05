# PhysicsGroup

## ```c#
Implements IHandle
```

## Summary

Represents a set ofPhysicsBodyobjects. Think ragdoll.
## Properties

```c#
float AngularDamping { set; } 
```
SetsPhysicsBody.AngularDampingon all bodies in this group.
```c#
Vector3 AngularVelocity { set; } 
```
SetsPhysicsBody.AngularVelocityon all bodies of this group.
```c#
IEnumerable<PhysicsBody> Bodies { get; } 
```
Returns all physics bodies that belong to this physics group.
```c#
int BodyCount { get; } 
```
Returns amount of physics bodies that belong to this physics group.
```c#
IEnumerable<PhysicsJoint> Joints { get; } 
```
Any and all joints that are attached to any body in this group.
```c#
float LinearDamping { set; } 
```
SetsPhysicsBody.LinearDampingon all bodies in this group.
```c#
float Mass { get; set; } 
```
The total mass of all thedynamicPhysicsBodiesin this group.
When setting the total mass, it will be set on each body proportionally to each of their old masses,
i.e. if a body had 25% of previous total mass, it will have 25% of new total mass.
```c#
Vector3 MassCenter { get; } 
```
Returns the center of mass for this group of physics bodies.
```c#
Vector3 Pos { get; } 
```
Returns position of the first physics body of this group, or zero vector if it has none.
```c#
bool Sleeping { get; set; } 
```
Physics bodies automatically go to sleep after a certain amount of time of inactivity to save on performance.
You can use this to wake the body up, or prematurely send it to sleep.
```c#
Vector3 Velocity { set; } 
```
SetsPhysicsBody.Velocityon all bodies of this group.
```c#
PhysicsWorld World { get; } 
```
The world in which this group belongs
## Methods

```c#
void AddAngularVelocity( Vector3 vel) 
```
Adds given amount of angular velocity to all physics bodies in this group.
```c#
void AddVelocity( Vector3 vel) 
```
Adds given amount of velocity (PhysicsBody.ApplyForce) to all physics bodies in this group.
```c#
void ApplyAngularImpulse( Vector3 vel, bool withMass = false) 
```
Adds given amount of angular linear impulse (PhysicsBody.ApplyAngularImpulse) to all physics bodies in this group.
```c#
void ApplyImpulse( Vector3 vel, bool withMass = false) 
```
Adds given amount of linear impulse (PhysicsBody.ApplyImpulse) to all physics bodies in this group.
```c#
PhysicsBody GetBody( int groupIndex) 
```
Gets aSandbox.PhysicsBodyat given index within this physics group. SeePhysicsGroup.BodyCount.
```c#
PhysicsBody GetBody( string groupName) 
```
Returns aSandbox.PhysicsBodyby itsPhysicsBody.GroupNamewithin this group.
```c#
void RebuildMass( ) 
```
CallsPhysicsBody.RebuildMasson all bodies of this group.
```c#
void Remove( ) 
```
Delete this group, and all of its bodies
```c#
void SetSurface( string name) 
```
Sets the physical properties of eachPhysicsShapeof this group.
