# IEntity

## 
```c#
Inherits IValid
```

## Summary

A generic entity.
## Properties

```c#
abstract Ray AimRay { get; } 
```
Get a ray representing where this entity is aiming. You can override this in your entity
to place the aim position at the entity's eye and the direction where it's looking.
```c#
abstract IClient Client { get; } 
```
The client that owns this entity, if any. Usually as a result of the entity being client's pawn, or being attached to the client's pawn.
```c#
abstract IComponentSystem Components { get; } 
```
Access to get, add and remove components
```c#
abstract int Id { get; } 
```
The entity's unique identifier, usually itsIEntity.NetworkIdent.
```c#
abstract bool IsAuthority { get; } 
```
Returns true if we have authority over this entity. This means we're either serverside,
or we're a clientside entity, or we're a serverside entity being predicted on the client.
```c#
abstract bool IsClientOnly { get; } 
```
True if this entity is a purely clientside entity, with no serverside components
```c#
abstract bool IsDormant { get; } 
```
Returns true if this entity is dormant (the client cannot see it, it isn't being networked)
```c#
abstract bool IsFromMap { get; } 
```
Returns true if this specific entity instance was spawned from the map.
```c#
abstract bool IsOwnedByLocalClient { get; } 
```
Clientside, whether theIEntity.Clientis the local client.
```c#
abstract int NetworkIdent { get; } 
```
The entity's network id. Client only entities have a network id too!
```c#
abstract IEntity Owner { get; } 
```
The entity that owns this entity. For example, a pawn's weapon will be owned by its pawn.
```c#
abstract IEntity Parent { get; } 
```
The parent entity.
```c#
abstract Vector3 Position { get; set; } 
```
The entity's world position
```c#
abstract Rotation Rotation { get; set; } 
```
The entity's world rotation
```c#
abstract string TagList { get; set; } 
```
List of tags this entity has, separated by spaces.
```c#
abstract Transform Transform { get; } 
```
Entity's transform from world origin.
```c#
abstract Vector3 Velocity { get; set; } 
```
The velocity in world coordinates.
```c#
abstract BBox WorldSpaceBounds { get; } 
```
Entity's axis-aligned bounding box (AABB) in world space.
## Methods

```c#
abstract void Delete( ) 
```
Delete this entity
## Extensions

```c#
void ClearWaterLevel( ) 
```
Clear any current water level. Pretend we're not in water anymore.
Usually called on Respawn.
```c#
float GetWaterLevel( ) 
```
Get the water level for this entity
