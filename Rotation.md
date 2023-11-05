# Rotation

## 
```c#
Implements IEquatable<Rotation>, IParsable<Rotation>
```

## Summary

Represents a Quaternion rotation. Can be interpreted as a direction unit vector (x,y,z) + rotation around the direction vector (w) which represents the up direction.
UnlikeAngles, this cannot store multiple revolutions around an axis.
## Constructors

```c#
Rotation( ) 
```
Initializes this rotation with all components set to zero.
```c#
Rotation( float x, float y, float z, float w) 
```
Initializes the rotation from given components.
```c#
Rotation( Vector3 v, float w) 
```
Initializes the rotation from a normal vector + rotation around it.
## Fields

```c#
static readonly Rotation Identity
```
A rotation that represents no rotation.
## Properties

```c#
static Rotation Random { get; } 
```
Returns a uniformly random rotation.
```c#
Vector3 Backward { get; } 
```
The backwards direction of this rotation.
```c#
Rotation Conjugate { get; } 
```
Returns conjugate of this rotation, meaning the X Y and Z components are negated.
```c#
Vector3 Down { get; } 
```
The downwards direction of this rotation.
```c#
Vector3 Forward { get; } 
```
The forwards direction of this rotation.
```c#
Rotation Inverse { get; } 
```
Returns the inverse of this rotation.
```c#
Vector3 Left { get; } 
```
The left hand direction of this rotation.
```c#
Rotation Normal { get; } 
```
Divides each component of the rotation by its length, normalizing the rotation.
```c#
Vector3 Right { get; } 
```
The right hand direction of this rotation.
```c#
Vector3 Up { get; } 
```
The upwards direction of this rotation.
```c#
float w { get; set; } 
```
The W component of this rotation (rotation around the normal defined by X,Y,Z components).
```c#
float x { get; set; } 
```
The X component of this rotation.
```c#
float y { get; set; } 
```
The Y component of this rotation.
```c#
float z { get; set; } 
```
The Z component of this rotation.
## Methods

```c#
static Rotation Difference( Rotation from, Rotation to) 
```
Returns the difference between two rotations, as a rotation
```c#
static Rotation From( Angles angles) 
```
Create a Rotation (quaternion) from Angles
```c#
static Rotation From( float pitch, float yaw, float roll) 
```
Create a Rotation (quaternion) from pitch yaw roll (degrees)
```c#
static Rotation FromAxis( Vector3 axis, float degrees) 
```
Create from angle and an axis
```c#
static Rotation FromPitch( float pitch) 
```
Create a Rotation (quaternion) from pitch (degrees)
```c#
static Rotation FromRoll( float roll) 
```
Create a Rotation (quaternion) from roll (degrees)
```c#
static Rotation FromYaw( float yaw) 
```
Create a Rotation (quaternion) from yaw (degrees)
```c#
static Rotation Lerp( Rotation a, Rotation b, float amount, bool clamp = true) 
```
Perform a linear interpolation from a to b by given amount.
```c#
static Rotation LookAt( Vector3 forward, Vector3 up) 
```
Create a Rotation (quaternion) from a forward and up vector
```c#
static Rotation LookAt( Vector3 forward) 
```
Create a Rotation (quaternion) from a forward and up vector
```c#
static Rotation Parse( string str) 
```
Given a string, try to convert this into a quaternion rotation. The format is "x,y,z,w"
```c#
static Rotation Parse( string str, IFormatProvider provider) 
```
ImplementsIParsable`1.ParseGiven a string, try to convert this into a quaternion rotation. The format is "x,y,z,w"
```c#
static Rotation Read( BinaryReader reader) 
```
Read a rotation from given binary reader.
```c#
static Rotation Slerp( Rotation a, Rotation b, float amount, bool clamp = true) 
```
Perform a spherical interpolation from a to b by given amount.
```c#
static bool TryParse( string str, out Rotation result) 
```
Given a string, try to convert this into a quaternion rotation. The format is "x,y,z,w"
```c#
static bool TryParse( string str, IFormatProvider provider, out Rotation result) 
```
ImplementsIParsable`1.TryParseGiven a string, try to convert this into a quaternion rotation. The format is "x,y,z,w"
```c#
float Angle( ) 
```
Returns the turn length of this rotation (from identity) in degrees
```c#
Angles Angles( ) 
```
Return this Rotation as pitch, yaw, roll angles
```c#
Rotation Clamp( Rotation to, float degrees) 
```
Clamp to within degrees of passed rotation
```c#
Rotation Clamp( Rotation to, float degrees, out float change) 
```
Clamp to within degrees of passed rotation. Also pases out the change in degrees, if any.
```c#
float Distance( Rotation to) 
```
The degree angular distance between this rotation and the target
```c#
float Pitch( ) 
```
Return this Rotation pitch
```c#
float Roll( ) 
```
Return this Rotation roll
```c#
Rotation RotateAroundAxis( Vector3 axis, float degrees) 
```
A convenience function that rotates this rotation around a given axis given amount of degrees
```c#
Rotation SmoothDamp( Rotation current, Rotation target, ref Vector3 velocity, float smoothTime, float deltaTime) 
```
Smoothly move towards the target rotation
```c#
void Write( BinaryWriter writer) 
```
Write this rotation to a System.IO.BinaryWriter.
```c#
float Yaw( ) 
```
Return this Rotation yaw
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( Rotation o) 
```
OverridesValueType.Equals
```c#
override int GetHashCode( ) 
```
OverridesValueType.GetHashCode
```c#
override string ToString( ) 
```
OverridesValueType.ToString
## Operators

```c#
Rotation +( Rotation a, Rotation b) 
```
No Summary
```c#
Rotation /( Rotation a, float f) 
```
No Summary
```c#
bool ==( Rotation left, Rotation right) 
```
No Summary
```c#
bool !=( Rotation left, Rotation right) 
```
No Summary
```c#
Vector3 *( Rotation f, Vector3 c1) 
```
No Summary
```c#
Rotation *( Rotation a, Rotation b) 
```
No Summary
```c#
Rotation *( Rotation a, float f) 
```
No Summary
```c#
Rotation -( Rotation a, Rotation b) 
```
No Summary
```c#
implicit Rotation =( Quaternion value) 
```
No Summary
```c#
implicit Quaternion =( Rotation value) 
```
No Summary
## Referencing Members

```c#
ModelBuilder = ModelBuilder.AddBone( string, Vector3, Rotation, string ) 
```
```c#
PhysicsShape = PhysicsBody.AddBoxShape( Vector3, Rotation, Vector3, bool ) 
```
```c#
ModelBuilder = ModelBuilder.AddCollisionBox( Vector3, Vector3?, Rotation? ) 
```
```c#
ModelBuilder = ModelBuilder.AddCollisionHull( Vector3[], Vector3?, Rotation? ) 
```
```c#
static void SandboxBaseExtensions.AddCube( VertexBuffer, Vector3, Vector3, Rotation, Color32 ) 
```
```c#
PhysicsShape = PhysicsBody.AddHullShape( Vector3, Rotation, List<Vector3>, bool ) 
```
```c#
PhysicsShape = PhysicsBody.AddHullShape( Vector3, Rotation, Span<Vector3>, bool ) 
```
```c#
Rotation = CitizenAnimationHelper.AimAngle { set; } 
```
```c#
void DebugOverlay.Axis( Vector3, Rotation, float, float, bool ) 
```
```c#
Bone.Bone( string, string, Vector3, Rotation ) 
```
```c#
void DebugOverlay.Box( Vector3, Rotation, Vector3, Vector3, Color, float, bool ) 
```
```c#
static void Breakables.Break( Model, Vector3, Rotation, float, Color, Result, PhysicsBody ) 
```
```c#
void DebugOverlay.Circle( Vector3, Rotation, float, Color, float, bool ) 
```
```c#
Rotation = ModelEntity.CollisionRotation { get; } 
```
```c#
static void SandboxBaseExtensions.CopyBonesFrom( Entity, Entity, Vector3, Rotation, float ) 
```
```c#
static Matrix = Matrix.CreateRotation( Rotation ) 
```
```c#
bool = GizmoControls.DragSquare( string, Vector2, Rotation, out Vector3, Action ) 
```
```c#
Rotation = Player.EyeLocalRotation { get; set; } 
```
```c#
Rotation = PawnController.EyeRotation { get; set; } 
```
```c#
Rotation = Player.EyeRotation { get; set; } 
```
```c#
Rotation = AnimatedEntity.GetAnimParameterRotation( string ) 
```
```c#
static Vector3 = Screen.GetDirection( Vector2, float, Rotation ) 
```
```c#
static Vector3 = Screen.GetDirection( Vector2, float, Rotation, Vector2 ) 
```
```c#
Rotation = SceneModel.GetRotation( string ) 
```
```c#
Rotation = PhysicsBody.InertiaRotation { get; } 
```
```c#
static PhysicsPoint = PhysicsPoint.Local( PhysicsBody, Vector3?, Rotation? ) 
```
```c#
Task<bool> = KeyframeEntity.LocalRotateKeyframeTo( Rotation, float, Function ) 
```
```c#
Rotation = PhysicsPoint.LocalRotation
```
```c#
virtual Rotation = Entity.LocalRotation { get; set; } 
```
```c#
override Rotation = ModelEntity.LocalRotation { get; set; } 
```
```c#
static Vector3 = Vector3.op_Multiply( Vector3, Rotation ) 
```
```c#
PhysicsPoint.PhysicsPoint( PhysicsBody, Vector3?, Rotation? ) 
```
```c#
static SceneObject = Decal.Place( SceneWorld, Material, Vector3, Rotation, Vector3, Color ) 
```
```c#
static void Decal.Place( To, DecalDefinition, Entity, int, Vector3, Rotation, Color ) 
```
```c#
static void Decal.Place( DecalDefinition, Entity, int, Vector3, Rotation ) 
```
```c#
static void Decal.Place( DecalDefinition, Entity, int, Vector3, Rotation, Color ) 
```
```c#
static void Decal.Place( DecalDefinition, Vector3, Rotation ) 
```
```c#
static void Decal.Place( DecalDefinition, Vector3, Rotation, Color ) 
```
```c#
bool = GizmoControls.Position( string, Vector3, out Vector3, Rotation?, float ) 
```
```c#
static Rotation = SandboxSystemExtensions.ReadRotation( BinaryReader ) 
```
```c#
BBox = BBox.Rotate( Rotation ) 
```
```c#
bool = GizmoControls.Rotate( string, Rotation, out Rotation ) 
```
```c#
Transform = Transform.RotateAround( Vector3, Rotation ) 
```
```c#
Vector3 = Vector3.RotateAround( Vector3, Rotation ) 
```
```c#
bool = GizmoControls.RotateSingle( string, Rotation, Color, out Rotation, float ) 
```
```c#
Rotation = Transform.Rotation
```
```c#
static Rotation = SandboxSystemExtensions.Rotation( Random ) 
```
```c#
Rotation = AsAccessor.Rotation { get; set; } 
```
```c#
static Rotation = Camera.Rotation { get; set; } 
```
```c#
abstract Rotation = IEntity.Rotation { get; set; } 
```
```c#
Rotation = PhysicsBody.Rotation { get; set; } 
```
```c#
Rotation = SceneCamera.Rotation { get; set; } 
```
```c#
Rotation = SceneObject.Rotation { get; set; } 
```
```c#
Rotation = Bone.Rotation { get; init; } 
```
```c#
virtual Rotation = Entity.Rotation { get; set; } 
```
```c#
override Rotation = ModelEntity.Rotation { get; set; } 
```
```c#
Rotation = InputMotionData.Rotation
```
```c#
Rotation = PawnController.Rotation { get; set; } 
```
```c#
Rotation = WorldPanel.Rotation { get; set; } 
```
```c#
Rotation = Transform.RotationToLocal( Rotation ) 
```
```c#
Rotation = Transform.RotationToLocal( Rotation ) 
```
```c#
Rotation = Transform.RotationToWorld( Rotation ) 
```
```c#
Rotation = Transform.RotationToWorld( Rotation ) 
```
```c#
static ScenePanel = SceneConstructor.ScenePanel( PanelCreator, SceneWorld, Vector3, Rotation, float, string ) 
```
```c#
SceneSunLight.SceneSunLight( SceneWorld, Rotation, Color ) 
```
```c#
static IDisposable = Gizmo.Scope( string, Vector3, Rotation, float ) 
```
```c#
void SceneModel.SetAnimParameter( string, Rotation ) 
```
```c#
void AnimatedEntity.SetAnimParameter( string, Rotation ) 
```
```c#
void SceneParticles.SetControlPoint( int, Rotation ) 
```
```c#
void Particles.SetOrientation( int, Rotation ) 
```
```c#
Rotation = Angles.ToRotation( ) 
```
```c#
Transform.Transform( Vector3, Rotation, float ) 
```
```c#
virtual bool = KeyframeEntity.TryLocalRotateTo( Rotation ) 
```
```c#
Rotation = RotationProperty.Value { get; set; } 
```
```c#
Rotation = ScenePortal.ViewRotation { get; set; } 
```
```c#
Transform = Transform.WithPosition( Vector3, Rotation ) 
```
```c#
Transform = Transform.WithRotation( Rotation ) 
```
```c#
static PhysicsPoint = PhysicsPoint.World( PhysicsBody, Vector3?, Rotation? ) 
```
```c#
static void SandboxSystemExtensions.Write( BinaryWriter, Rotation ) 
```
