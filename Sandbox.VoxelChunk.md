# VoxelChunk

## 
```c#
Derives from ModelEntity
```

## Summary

OverridesEntity.ClientSpawnCalled when the entity spawns on client.
## Constructors

```c#
VoxelChunk( ) 
```
No Summary
## Properties

```c#
VoxelSurface ParentSurface { get; set; } 
```
No Summary
## Methods

```c#
void BreakLocalSpace( int x, int y) 
```
No Summary
```c#
void BreakLocalSpace( int localX, int localY, int radius) 
```
No Summary
```c#
void BreakWorldSpace( Vector3 position) 
```
No Summary
```c#
void CreateModel( Vector2 size, Vector2 offset, int width, int height, float thickness, string material, bool frozen, byte[] data = null, int blockCount = 0) 
```
No Summary
```c#
bool IsBlockEmpty( int x, int y) 
```
No Summary
```c#
bool IsBlockInBounds( int x, int y) 
```
No Summary
```c#
bool IsBlockOutOfBounds( int x, int y) 
```
No Summary
```c#
bool IsBlockSolid( int x, int y) 
```
No Summary
```c#
void MarkForDeletion( ) 
```
No Summary
```c#
protected void OnClientTick( ) 
```
No Summary
```c#
protected void OnServerTick( ) 
```
No Summary
```c#
void QueueSplit( BlockPosition[] positions, int x, int y, int width, int height) 
```
No Summary
```c#
void SetBlockEmpty( int x, int y) 
```
No Summary
```c#
void SetBlockSolid( int x, int y) 
```
No Summary
```c#
override void ClientSpawn( ) 
```
OverridesEntity.ClientSpawnCalled when the entity spawns on client.
```c#
protected override void OnPhysicsCollision( CollisionEventData eventData) 
```
OverridesEntity.OnPhysicsCollisionCalled when this entity collides with anything else via Physics.
```c#
override void TakeDamage( DamageInfo info) 
```
OverridesEntity.TakeDamageCalled when the entity receives a damage event. This is where you want to subtract health, etc.
## Nested Types

