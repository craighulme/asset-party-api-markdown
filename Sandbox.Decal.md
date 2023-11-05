# Decal

## 
```c#
Derives from object
```

## Summary

A library to allow the management of decals in the world
## Methods

```c#
static void Clear( bool world, bool entities) 
```
Clear all decals from the world or entities
```c#
static void Clear( To toTarget, bool world, bool entities) 
```
Clear all decals from the world or entities
```c#
static void Move( Entity source, Entity dest) 
```
Move decals from one entity to another
```c#
static void Move( To toTarget, Entity source, Entity dest) 
```
Move decals from one entity to another
```c#
static SceneObject Place( SceneWorld world, Material material, Vector3 position, Rotation rotation, Vector3 scale, Color color) 
```
Places a decal in aSandbox.SceneWorldWill throw an assert if called outside of GameMenu
```c#
static void Place( To toTarget, DecalDefinition decal, Entity ent, int bone, Vector3 position, Rotation rotation, Color color) 
```
Place this decal somewhere on an entity, if it's valid. If it isn't valid, we'll stick it on the world.
```c#
static void Place( DecalDefinition decal, Entity ent, int bone, Vector3 position, Rotation rotation) 
```
Place this decal somewhere on an entity, if it's valid. If it isn't valid, we'll stick it on the world.
```c#
static void Place( DecalDefinition decal, Entity ent, int bone, Vector3 position, Rotation rotation, Color color) 
```
Place this decal somewhere on an entity, if it's valid. If it isn't valid, we'll stick it on the world.
```c#
static void Place( DecalDefinition decal, TraceResult tr) 
```
Place this decal somewhere
```c#
static void Place( DecalDefinition decal, TraceResult tr, Color color) 
```
Place this decal somewhere
```c#
static void Place( DecalDefinition decal, Vector3 position, Rotation rotation) 
```
Place this decal somewhere (on the world)
```c#
static void Place( DecalDefinition decal, Vector3 position, Rotation rotation, Color color) 
```
Place this decal somewhere (on the world)
