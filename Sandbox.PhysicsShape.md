# PhysicsShape

## 
```c#
Implements IHandle
```

## Summary

Represents a basic, convex shape. APhysicsBodyconsists of one or more of these.
## Properties

```c#
PhysicsBody Body { get; } 
```
The physics body we belong to.
```c#
object Collider { get; set; } 
```
The collider object that created / owns this shape
```c#
bool EnableSolidCollisions { get; set; } 
```
Controls whether this shape has solid collisions.
```c#
bool EnableTouch { get; set; } 
```
Controls whether this shape can fire touch events for its owning entity. (Entity.StartTouch, Touch and EndTouch)
```c#
bool EnableTouchPersists { get; set; } 
```
Controls whether this shape can fire continuous touch events for its owning entity (i.e. calling Entity.Touch every frame)
```c#
bool EnableTraceAndQueries { get; set; } 
```
Controls whether traces and entity queries (e.g. Entity.FindInBox) can hit/detect this shape.
```c#
bool IsCapsuleShape { get; } 
```
Is this a CapsuleShape
```c#
bool IsHullShape { get; } 
```
Is this a HullShape
```c#
bool IsMeshShape { get; } 
```
Is this a MeshShape
```c#
bool IsSphereShape { get; } 
```
Is this a SphereShape
```c#
bool IsTrigger { get; set; } 
```
If true, then this collider isn't solid
```c#
Vector3 Scale { get; } 
```
Returns the scale of this object. (Most of the time inherited from owning entity's scale)
```c#
Surface Surface { get; set; } 
```
No Summary
```c#
string SurfaceMaterial { get; set; } 
```
Controls physical properties of this shape.
## Methods

```c#
bool AddTag( string tag) 
```
Add a tag to this shape.
```c#
bool ClearTags( ) 
```
Clear all tags from this shape.
```c#
void DisableAllCollision( ) 
```
Disable contact, trace and touch
```c#
void EnableAllCollision( ) 
```
Enable contact, trace and touch
```c#
bool HasTag( string tag) 
```
Does this shape have a specific tag?
```c#
void Remove( ) 
```
Remove this shape. After calling this the shape should be considered released and not used again.
```c#
bool RemoveTag( string tag) 
```
Remove a tag from this shape.
```c#
void UpdateMesh( List<Vector3> vertices, List<int> indices) 
```
Recreate the collision mesh (Only if this physics shape is type Mesh)
```c#
void UpdateMesh( Span<Vector3> vertices, Span<int> indices) 
```
Recreate the collision mesh (Only if this physics shape is type Mesh)
