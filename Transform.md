# Transform

## ```c#
Implements IEquatable<Transform>
```

## Summary

A struct containing a position, rotation and scale. This is commonly used in engine to describe
entity position, bone position and scene object position.
## Constructors

```c#
Transform( Vector3 pos = null) 
```
No Summary
```c#
Transform( Vector3 position, Rotation rotation, float scale = 1) 
```
No Summary
## Fields

```c#
static readonly Transform Zero
```
Represents a zero transform, that being, a transform with scale of 1, position ofVector3.Zeroand rotation ofRotation.Identity.
```c#
Vector3 Position
```
Position of the transform.
```c#
Rotation Rotation
```
Rotation of this transform.
```c#
float Scale
```
Scale of the transform. Does not itself scaleTransform.PositionorTransform.Rotation.
## Properties

```c#
Vector3 Backward { get; } 
```
No Summary
```c#
Vector3 Down { get; } 
```
No Summary
```c#
Vector3 Forward { get; } 
```
No Summary
```c#
Vector3 Left { get; } 
```
No Summary
```c#
Vector3 Right { get; } 
```
No Summary
```c#
Vector3 Up { get; } 
```
No Summary
## Methods

```c#
static Transform Concat( Transform parent, Transform local) 
```
Concatenate (add together) the 2 given transforms and return a new resulting transform.
```c#
static Transform Lerp( Transform a, Transform b, float t, bool clamp) 
```
Perform linear interpolation from one transform to another.
```c#
static Transform Parse( string str) 
```
Given a string, try to convert this into a transform. The format is"px,py,pz,rx,ry,rz,rw".
```c#
static Transform Read( BinaryReader reader) 
```
Read a transform from given binary reader.
```c#
Transform Add( Vector3 position, bool worldSpace) 
```
Add a position to this transform and return the result.
```c#
Vector3 NormalToLocal( Vector3 worldNormal) 
```
Convert a world normal to a local normal
```c#
Vector3 NormalToWorld( Vector3 localNormal) 
```
Convert a local normal to a world normal
```c#
Vector3 PointToLocal( Vector3 worldPoint) 
```
Convert a point in world space to a point in this transform's local space
```c#
Vector3 PointToWorld( Vector3 localPoint) 
```
Convert a point in this transform's local space to a point in world space
```c#
Transform RotateAround( Vector3 center, Rotation rot) 
```
Rotate this transform around given point by given rotation and return the result.
```c#
Rotation RotationToLocal( Rotation worldRot) 
```
Convert a world rotation to a local rotation
```c#
Rotation RotationToWorld( Rotation localRotation) 
```
Convert a local rotation to a world rotation
```c#
Transform ToLocal( Transform child) 
```
Convert child transform from the world to a local transform
```c#
Transform ToWorld( Transform child) 
```
Convert child transform from local to the world
```c#
Vector3 TransformVector( Vector3 local) 
```
Transform a Vector as if it were a child of this transform
```c#
Transform WithPosition( Vector3 position) 
```
Return this transform with a new position.
```c#
Transform WithPosition( Vector3 position, Rotation rotation) 
```
Return this transform with a new position and rotation
```c#
Transform WithRotation( Rotation rotation) 
```
Return this transform with a new rotation.
```c#
Transform WithScale( float scale) 
```
Return this transform with a new scale.
```c#
void Write( BinaryWriter writer) 
```
Write this transform to a System.IO.BinaryWriter.
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( Transform o) 
```
OverridesValueType.Equals
```c#
override int GetHashCode( ) 
```
OverridesValueType.GetHashCode
```c#
override string ToString( ) 
```
OverridesValueType.ToStringFormats the Transform into a string "pos, rot, scale"
## Operators

```c#
bool ==( Transform left, Transform right) 
```
No Summary
```c#
bool !=( Transform left, Transform right) 
```
No Summary
## Referencing Members

```c#
PhysicsShape = PhysicsBody.AddShape( HullPart, Transform, bool ) 
```
```c#
PhysicsShape = PhysicsBody.AddShape( MeshPart, Transform, bool, bool ) 
```
```c#
static Transform = VR.Anchor { get; set; } 
```
```c#
bool = PhysicsBody.CheckOverlap( PhysicsBody, Transform ) 
```
```c#
FootstepEvent.FootstepEvent( int, Transform, float, string ) 
```
```c#
Transform? = Model.GetAttachment( string ) 
```
```c#
Transform? = Model.GetAttachment( int ) 
```
```c#
Transform? = SceneModel.GetAttachment( string, bool ) 
```
```c#
Transform? = ModelEntity.GetAttachment( string, bool ) 
```
```c#
Transform = Model.GetBoneTransform( int ) 
```
```c#
Transform = Model.GetBoneTransform( string ) 
```
```c#
Transform = ModelEntity.GetBoneTransform( int, bool ) 
```
```c#
Transform = ModelEntity.GetBoneTransform( string, bool ) 
```
```c#
Transform = SceneModel.GetBoneWorldTransform( int ) 
```
```c#
Transform = SceneModel.GetBoneWorldTransform( string ) 
```
```c#
Transform = VrInput.Head { get; } 
```
```c#
Transform = ShatterGlass.InitialTransform { get; } 
```
```c#
Task<bool> = KeyframeEntity.KeyframeTo( Transform, float, Function ) 
```
```c#
static Transform? = Sound.Listener { get; set; } 
```
```c#
Transform = PhysicsPoint.LocalTransform { get; } 
```
```c#
virtual Transform = Bone.LocalTransform { get; } 
```
```c#
SceneObject = GizmoDraw.Model( string, Transform ) 
```
```c#
SceneObject = GizmoDraw.Model( Model, Transform ) 
```
```c#
void PhysicsBody.Move( Transform, float ) 
```
```c#
static IDisposable = Gizmo.ObjectScope<T,>( T, Transform ) 
```
```c#
void GizmoDraw.Particles( string, Transform, float? ) 
```
```c#
static Transform = SandboxSystemExtensions.ReadTransform( BinaryReader ) 
```
```c#
static void Graphics.Render( SceneObject, Transform?, Color?, Material ) 
```
```c#
SceneCullingBox.SceneCullingBox( SceneWorld, Transform, Vector3, CullMode ) 
```
```c#
SceneFogVolume.SceneFogVolume( SceneWorld, Transform, BBox, float, float ) 
```
```c#
SceneModel.SceneModel( SceneWorld, string, Transform ) 
```
```c#
SceneModel.SceneModel( SceneWorld, Model, Transform ) 
```
```c#
SceneObject.SceneObject( SceneWorld, Model, Transform ) 
```
```c#
SceneObject.SceneObject( SceneWorld, string, Transform ) 
```
```c#
ScenePortal.ScenePortal( SceneWorld, Model, Transform, bool, int ) 
```
```c#
static IDisposable = Gizmo.Scope( string, Transform ) 
```
```c#
void AnimatedEntity.SetAnimParameter( string, Transform ) 
```
```c#
void ModelEntity.SetBone( int, Transform ) 
```
```c#
void ModelEntity.SetBone( string, Transform ) 
```
```c#
bool = ModelEntity.SetBoneTransform( int, Transform, bool ) 
```
```c#
bool = ModelEntity.SetBoneTransform( string, Transform, bool ) 
```
```c#
void SceneModel.SetBoneWorldTransform( int, Transform ) 
```
```c#
void SceneParticles.SetControlPoint( int, Transform ) 
```
```c#
void Particles.SetEntityBone( int, Entity, int, Transform, bool ) 
```
```c#
void VROverlay.SetHudTransform( Transform ) 
```
```c#
virtual void Entity.SetParent( Entity, string, Transform? ) 
```
```c#
virtual void Entity.SetParent( Entity, int, Transform? ) 
```
```c#
void VROverlay.SetTransformAbsolute( Transform ) 
```
```c#
void VROverlay.SetTransformRelative( VROverlay, Transform ) 
```
```c#
void VROverlay.SetTransformRelative( VRTrackedDevice, Transform ) 
```
```c#
PhysicsGroup = PhysicsWorld.SetupPhysicsFromModel( Model, Transform, PhysicsMotionType ) 
```
```c#
void GizmoDraw.Text( string, Transform, string, float, TextFlag ) 
```
```c#
BBox = BBox.Transform( Transform ) 
```
```c#
abstract Transform = IEntity.Transform { get; } 
```
```c#
static Transform = Gizmo.Transform { get; set; } 
```
```c#
Transform = PhysicsBody.Transform { get; set; } 
```
```c#
Transform = CubemapFogController.Transform { get; set; } 
```
```c#
Transform = SceneCullingBox.Transform { get; set; } 
```
```c#
Transform = SceneFogVolume.Transform { get; set; } 
```
```c#
Transform = SceneObject.Transform { get; set; } 
```
```c#
Transform = PhysicsPoint.Transform { get; } 
```
```c#
Transform = BodyPart.Transform { get; init; } 
```
```c#
Transform = FootstepEvent.Transform { get; set; } 
```
```c#
abstract Transform = EntityObject.Transform { get; set; } 
```
```c#
Transform = Result.Transform { get; set; } 
```
```c#
virtual Transform = Entity.Transform { get; set; } 
```
```c#
Transform = VROverlay.Transform { get; set; } 
```
```c#
Transform = VrHand.Transform { get; } 
```
```c#
Transform = TrackedObject.Transform { get; } 
```
```c#
Transform = WorldPanel.Transform { get; set; } 
```
```c#
virtual bool = KeyframeEntity.TryKeyframeTo( Transform ) 
```
```c#
void GizmoDraw.WorldText( string, Transform, string, float, TextFlag ) 
```
```c#
static void SandboxSystemExtensions.Write( BinaryWriter, Transform ) 
```
