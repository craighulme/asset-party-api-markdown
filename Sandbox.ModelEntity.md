# ModelEntity

## ```c#
Derives from Entity
```

## Summary

A generic entity that is capable rendering a model and have physics.
## Constructors

```c#
ModelEntity( ) 
```
No Summary
```c#
ModelEntity( string modelName) 
```
No Summary
```c#
ModelEntity( string modelName, Entity parent) 
```
No Summary
## Properties

```c#
virtual SceneObject SceneObject { get; } 
```
TheModelEntity.SceneObjectthat represents this entity.
```c#
int BoneCount { get; } 
```
Number of bones model of this entity has.
```c#
BBox CollisionBounds { get; set; } 
```
The collision bounds.
```c#
Vector3 CollisionPosition { get; } 
```
Position of the collision model. Will be same asModelEntity.Positionin most cases.
```c#
Rotation CollisionRotation { get; } 
```
Rotation of the collision model. Will be same asModelEntity.Rotationin most cases.
```c#
Vector3 CollisionWorldSpaceCenter { get; } 
```
Center of the collision model (OBB) in world-space coordinates. Will be same asEntity.WorldSpaceBounds.Center in most cases.
```c#
bool EnableAllCollisions { set; } 
```
Enable or disableModelEntity.EnableSolidCollisions,ModelEntity.EnableTraceAndQueriesandModelEntity.EnableTouchat once.
```c#
bool EnableHitboxes { get; set; } 
```
Use hitboxes for traces etc.
```c#
bool EnableSelfCollisions { set; } 
```
Allow ragdoll parts to collide with each other.
```c#
bool EnableShadowCasting { get; set; } 
```
ImplementsEntity.EnableShadowCastingDon't cast no shadow.
```c#
bool EnableSolidCollisions { get; set; } 
```
Enables or disables solid collisions (as in, affects only physics collisions, not trace and touch events) between this and other entities.This value will propagate to all childPhysicsBodies.
```c#
bool EnableTouch { get; set; } 
```
Decides whetherEntity.StartTouch,Entity.TouchandEntity.EndTouchcallbacks are allowed to be called.This value will propagate to all childPhysicsBodies.Touch events are propagated to parent entities on the server!
```c#
bool EnableTouchPersists { get; set; } 
```
Continuously callEntity.Touchfor each entity that is touching us, rather than once on touch start.
This value will propagate to all childPhysicsBodies.
```c#
bool EnableTraceAndQueries { get; set; } 
```
Allow or disallow traces to hit this entity, and for entity queries (e.g. Entity.FindInBox) to detect it.
This value will propagate to all childPhysicsBodies.
```c#
string HitboxSet { get; set; } 
```
The currently active hitbox set.
```c#
int MaterialGroupCount { get; } 
```
Returns the material group count of this entity's model.
```c#
Model Model { get; set; } 
```
Access to this entity's model.
```c#
MorphCollection Morphs { get; } 
```
Access this entity's morph collection. Morphs are generally used in the model to control
the face, for things like emotions and lip sync.
```c#
PhysicsBody PhysicsBody { get; } 
```
The first PhysicsBody of this entity, if there is one, for convenience purposes.
To access otherPhysicsBodies, usePhysicsGroup
```c#
bool PhysicsEnabled { get; set; } 
```
Enable or disable physics motion.
```c#
Color RenderColor { get; set; } 
```
Color tint for this entity.
```c#
string SceneLayer { set; } 
```
No Summary
```c#
SurroundingBoundsType SurroundingBoundsMode { get; set; } 
```
Set the method used to work out the surrounding bounds. The bounds are important for
traces and collision checks, because they're used the quickly eliminate collisions.AffectsEntity.WorldSpaceBounds.
```c#
bool UsePhysicsCollision { set; } 
```
Enable physics collisions for this entity. Input value is ignored. This is set automatically when setting up physics from a model.
```c#
override Vector3 LocalPosition { get; set; } 
```
OverridesEntity.LocalPositionThe entity's position relative to its parent (or the world if no parent)
```c#
override Rotation LocalRotation { get; set; } 
```
OverridesEntity.LocalRotationThe entity's local rotation
```c#
override Vector3 Position { get; set; } 
```
OverridesEntity.PositionThe entity's world position
```c#
override Rotation Rotation { get; set; } 
```
OverridesEntity.RotationThe entity's world rotation
```c#
override Vector3 Velocity { get; set; } 
```
OverridesEntity.VelocityThe velocity in world coordinates.
## Methods

```c#
virtual void OnAnimEventFootstep( Vector3 position, int foot, float volume) 
```
Called when the model fires a specific animation event for footsteps. (AE_FOOTSTEP)
```c#
virtual void OnAnimEventGeneric( string name, int intData, float floatData, Vector3 vectorData, string stringData) 
```
Called when the entity's model files an animation event.
```c#
virtual void OnNewModel( Model model) 
```
Called when the model of this entity has changed.
```c#
virtual void PhysicsClear( ) 
```
Destroy all physics objects.
```c#
void ClearMaterialOverride( ) 
```
Clear all material replacements.
```c#
Transform[] ComputeBones( float timeOffset) 
```
Returns all bone transforms. Clientside, the bones will be interpolated. This is mostly useful for clientside ragdoll creation.
```c#
void CopyBodyGroups( ModelEntity from) 
```
Copy body groups from a given model entity. They will be copied by id, so it's best that both entities have the same model.
```c#
void CopyFrom( ModelEntity entity) 
```
Copy the model settings from another model entity. This is most useful when creating things such as
ragdolls. This copies model, decals, body groups, material groups, material overrides.
```c#
void CopyMaterialGroup( ModelEntity from) 
```
Copy material group over to this model by its id.
```c#
void CopyMaterialOverrides( ModelEntity from) 
```
Copy material replacements from given entity.
```c#
Transform? GetAttachment( string name, bool worldspace = true) 
```
Returns transform of given attachment by name.
```c#
int GetBone( PhysicsBody body) 
```
Get the bone that this physics body is attached to.
```c#
int GetBoneIndex( string boneName) 
```
Returns bone index for given bone name.
```c#
string GetBoneName( int bone) 
```
Returns name of the bone at given index.
```c#
int GetBoneParent( int bone) 
```
Returns index of the parent bone of the bone at given index.
```c#
int GetBoneParent( string boneName) 
```
Returns index of the parent bone of given bone by name.
```c#
PhysicsBody GetBonePhysicsBody( int iBone) 
```
Get the physics body attached to this bone.
```c#
Transform GetBoneTransform( int bone, bool worldspace = true) 
```
Returns the current transform of a given bone.
```c#
Transform GetBoneTransform( string boneName, bool worldspace = true) 
```
Returns the current transform of a given bone by name.
```c#
int GetMaterialGroup( ) 
```
Get currently active material group id.
```c#
string GetModelName( ) 
```
Returns the name (filepath) of the model of this entity.
```c#
void ResetBone( int bone) 
```
Reset visual bone transform override, by bone index.
```c#
void ResetBone( string name) 
```
Reset visual bone transform override, by bone name.
```c#
void ResetBones( ) 
```
Reset all bone transform overrides.
```c#
void SetBodyGroup( int group, int value) 
```
Set body group to replace parts of the model by bodygroup index.
```c#
void SetBodyGroup( string group, int value) 
```
Set body group to replace parts of the model by bodygroup name.This is useful when multiple models are meant to have same body groups, such as player models.
```c#
void SetBone( int bone, Transform tx) 
```
Set visual bone transform override, by bone index.
```c#
void SetBone( string name, Transform tx) 
```
Set visual bone transform override, by bone name.
```c#
bool SetBoneTransform( int bone, Transform tx, bool worldspace = true) 
```
Sets transform of a physics bone, by bone index. (ModelEntity.PhysicsBodyassociated with this bone, if any)
```c#
bool SetBoneTransform( string boneName, Transform tx, bool worldspace = true) 
```
Sets transform of a physics bone, by bone name. (ModelEntity.PhysicsBodyassociated with this bone, if any)
```c#
void SetMaterialGroup( int group) 
```
Set material group to replace materials of the model by material group index.
```c#
void SetMaterialGroup( string group) 
```
Set material group to replace materials of the model by material group name.
```c#
void SetMaterialOverride( Material material) 
```
Replaces all materials on the model with the given material.
```c#
void SetMaterialOverride( string materialPath) 
```
Replaces all materials on the model with the given material by name.
```c#
void SetMaterialOverride( Material material, string attributeName) 
```
Replaces all materials of the model that have the givenUser Material Attributeset to"1", with given material.The system checks both the models' default material group materials and the materials of the active material group.
```c#
void SetModel( string name) 
```
Set theModelEntity.Modelof this entity by name/path.
```c#
PhysicsGroup SetupPhysicsFromAABB( PhysicsMotionType motionType, Vector3 mins, Vector3 maxs) 
```
Clears all physics bodies and sets up physics from givenAABBthat is always upright.
Requires non dynamic motion type.
```c#
PhysicsGroup SetupPhysicsFromCapsule( PhysicsMotionType motionType, Capsule capsule) 
```
Clears all physics bodies and sets up physics as a capsule that is always upright. A capsule is a cylinder with round ends.
Requires non dynamic motion type.
```c#
PhysicsGroup SetupPhysicsFromCylinder( PhysicsMotionType motionType, Capsule capsule) 
```
Clears all physics bodies and sets up physics as a cylinder that is always upright.
Requires non dynamic motion type.
```c#
PhysicsGroup SetupPhysicsFromModel( PhysicsMotionType motionType, bool startasleep = false) 
```
Clears all physics bodies and sets up physics from the model's data as set up in ModelDoc.
```c#
PhysicsGroup SetupPhysicsFromOBB( PhysicsMotionType motionType, Vector3 mins, Vector3 maxs) 
```
Clears all physics bodies and sets up physics from givenOBB.
```c#
PhysicsGroup SetupPhysicsFromOrientedCapsule( PhysicsMotionType motionType, Capsule capsule) 
```
Clears all physics bodies and sets up physics as a capsule. A capsule is a cylinder with round ends.
```c#
PhysicsGroup SetupPhysicsFromSphere( PhysicsMotionType motionType, Vector3 center, float radius) 
```
Clears all physics bodies and sets up physics as a single sphere.
```c#
void TakeDecalsFrom( ModelEntity source) 
```
Move all of the decals from this entity onto ourself
## Inheriting Types

