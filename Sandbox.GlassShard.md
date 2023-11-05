# GlassShard

## ```c#
Derives from ModelEntity
```

## Summary

A procedurally shattering glass shard.
## Constructors

```c#
GlassShard( ) 
```
No Summary
## Properties

```c#
Material Material { get; set; } 
```
No Summary
```c#
ShatterGlass ParentPanel { get; set; } 
```
No Summary
```c#
GlassShard ParentShard { get; set; } 
```
No Summary
```c#
Vector2 StressPosition { get; set; } 
```
No Summary
```c#
Vector3 StressVelocity { get; set; } 
```
No Summary
## Methods

```c#
void AddVertex( Vector2 vertex) 
```
No Summary
```c#
protected void ClientTick( ) 
```
No Summary
```c#
void Freeze( ) 
```
No Summary
```c#
bool GenerateShardModel( ) 
```
No Summary
```c#
Model GenerateShardModel( out Vector2 localPanelSpaceOrigin) 
```
No Summary
```c#
Vector2 GetPanelVertexAverage( ) 
```
No Summary
```c#
bool IsFrozen( ) 
```
No Summary
```c#
bool IsOnFrameEdge( ) 
```
No Summary
```c#
bool IsShardNearPanelSpacePosition( ) 
```
No Summary
```c#
void MarkForDeletion( ) 
```
No Summary
```c#
protected void OnServerTick( ) 
```
No Summary
```c#
bool ShatterLocalSpace( Vector2 position) 
```
No Summary
```c#
void ShatterWorldSpace( Vector3 position) 
```
No Summary
```c#
Vector3 TransformPosPanelToWorld( Vector2 position) 
```
No Summary
```c#
Vector2 TransformPosWorldToPanel( Vector3 position) 
```
No Summary
```c#
protected void TryGenerateShardModel( ) 
```
No Summary
```c#
void TryGenerateShardModel( Vector3 vShatterPos, Vector3 vShatterVel, bool bVelocity, bool bFreeze = false) 
```
No Summary
```c#
void Unfreeze( ) 
```
No Summary
```c#
override void ClientSpawn( ) 
```
OverridesEntity.ClientSpawnCalled when the entity spawns on client.
```c#
protected override void OnDestroy( ) 
```
OverridesEntity.OnDestroyCalled when the entity was destroyed. This is not the same as the class destructor.
```c#
protected override void OnPhysicsCollision( CollisionEventData eventData) 
```
OverridesEntity.OnPhysicsCollisionCalled when this entity collides with anything else via Physics.
```c#
override void TakeDamage( DamageInfo info) 
```
OverridesEntity.TakeDamageCalled when the entity receives a damage event. This is where you want to subtract health, etc.
```c#
override void Touch( Entity other) 
```
OverridesEntity.TouchAn entity has touched this trigger entity. RequiresEnableTouchenabled on this entity.See alsoModelEntity.EnableTouchPersists.
