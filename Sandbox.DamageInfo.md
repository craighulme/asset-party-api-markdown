# DamageInfo

## 
```c#
Derives from ValueType
```

## Summary

The player or NPC or exploding barrel (etc)1 that is attacking
## Properties

```c#
Entity Attacker { get; set; } 
```
The player or NPC or exploding barrel (etc)1 that is attacking
```c#
PhysicsBody Body { get; set; } 
```
The physics body that was hit
```c#
int BoneIndex { get; set; } 
```
The bone index that the hitbox was attached to
```c#
float Damage { get; set; } 
```
The actual amount of damage this attack causes
```c#
Vector3 Force { get; set; } 
```
The force of the damage - for moving physics etc. This would be the trajectory
of the bullet multiplied by the speed and mass.
```c#
Hitbox Hitbox { get; set; } 
```
The hitbox (if any) that was hit
```c#
Vector3 Position { get; set; } 
```
The position the damage is being inflicted (the bullet entry point)
```c#
HashSet<string> Tags { get; set; } 
```
Damage tags, extra information about this attack
```c#
Entity Weapon { get; set; } 
```
The weapon that the attacker is using
## Methods

```c#
static DamageInfo FromBullet( Vector3 hitPosition, Vector3 hitForce, float damage) 
```
Creates a new DamageInfo with the "bullet" tag
```c#
static DamageInfo FromExplosion( Vector3 sourcePosition, Vector3 force, float damage) 
```
Creates a new DamageInfo with the "explosion" tag
```c#
static DamageInfo Generic( float damage) 
```
Creates a new DamageInfo with no tags
```c#
bool HasAllTags( string[] tags) 
```
Returns true if this DamageInfo has ALL of the following tags
```c#
bool HasAnyTag( string[] tags) 
```
Returns true if this DamageInfo has ANY of the following tags
```c#
bool HasTag( string tag) 
```
Do we have a tag that matches this string?
```c#
DamageInfo UsingTraceResult( TraceResult result) 
```
Fills in the PhysicsBody and Hitbox from the trace result
```c#
DamageInfo WithAttacker( Entity attacker, Entity weapon = null) 
```
Set the attacker
```c#
DamageInfo WithBone( int bone) 
```
Sets the bone index
```c#
DamageInfo WithDamage( float damage) 
```
Sets the amount of damage
```c#
DamageInfo WithForce( Vector3 force) 
```
Sets the force
```c#
DamageInfo WithHitBody( PhysicsBody body) 
```
Sets the hit physics body
```c#
DamageInfo WithPosition( Vector3 position) 
```
Sets the position
```c#
DamageInfo WithTag( string tag) 
```
Includes one tag to this damage info.
Can be accessed viaDamageInfo.HasTagandDamageInfo.Tagsfor a full list.
```c#
DamageInfo WithTags( string[] tags) 
```
Includes any number of tags to this damage info.
Can be accessed viaDamageInfo.HasTagandDamageInfo.Tagsfor a full list.
```c#
DamageInfo WithWeapon( Entity weapon) 
```
Set the attacker
## Referencing Members

```c#
protected void BasePhysics.ApplyDamageForces( DamageInfo ) 
```
```c#
void Result.CopyParamsFrom( DamageInfo ) 
```
```c#
static void SandboxBaseExtensions.ProceduralHitReaction( AnimatedEntity, DamageInfo, float ) 
```
```c#
virtual void Entity.TakeDamage( DamageInfo ) 
```
```c#
override void BasePhysics.TakeDamage( DamageInfo ) 
```
```c#
override void GlassShard.TakeDamage( DamageInfo ) 
```
```c#
override void VoxelChunk.TakeDamage( DamageInfo ) 
```
```c#
override void Water.TakeDamage( DamageInfo ) 
```
```c#
override void AnimatedMapEntity.TakeDamage( DamageInfo ) 
```
```c#
override void BrushEntity.TakeDamage( DamageInfo ) 
```
```c#
override void ButtonEntity.TakeDamage( DamageInfo ) 
```
```c#
override void DoorEntity.TakeDamage( DamageInfo ) 
```
```c#
override void PhysicsBrushEntity.TakeDamage( DamageInfo ) 
```
```c#
override void Prop.TakeDamage( DamageInfo ) 
```
```c#
override void Player.TakeDamage( DamageInfo ) 
```
