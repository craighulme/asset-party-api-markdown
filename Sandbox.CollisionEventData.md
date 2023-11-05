# CollisionEventData

## ```c#
Derives from ValueType
```

## Summary

The collision data involving two entities, this is used inEntity.OnPhysicsCollision.
Each Entity receives this callback with theThisandOtherswapped.
## Fields

```c#
Vector3 Normal
```
Direction perpendicular to our hit surface.
```c#
CollisionEntityData Other
```
The other entity data that was involved in this collision.
```c#
Vector3 Position
```
The point at which the collision contact happened.
```c#
float Speed
```
Collision speed.
```c#
CollisionEntityData This
```
Our entity data from the collision.
```c#
Vector3 Velocity
```
Speed of the contact. speed of surface 1 relative to surface 0
## Referencing Members

```c#
protected virtual void Entity.OnPhysicsCollision( CollisionEventData ) 
```
```c#
protected override void BasePhysics.OnPhysicsCollision( CollisionEventData ) 
```
```c#
protected override void GlassShard.OnPhysicsCollision( CollisionEventData ) 
```
```c#
protected override void VoxelChunk.OnPhysicsCollision( CollisionEventData ) 
```
```c#
protected override void Prop.OnPhysicsCollision( CollisionEventData ) 
```
