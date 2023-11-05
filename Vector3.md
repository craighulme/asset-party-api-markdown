# Vector3

## Derives from ValueType
Implements IEquatable< Vector3>, IParsable< Vector3>

## Summary

A point in 3D space.
## Constructors

```c#
Vector3( float x, float y, float z) 
```
Initializes a vector with given components.
```c#
Vector3( float x, float y) 
```
Initializes a vector with given components and Z set to 0.
```c#
Vector3( Vector3 other) 
```
Initializes a vector3 from a given vector3, i.e. a copy.
```c#
Vector3( Vector2 other, float z) 
```
Initializes a vector3 from given vector2 and the given Z component.
```c#
Vector3( float all = 0) 
```
Initializes the vector with all components set to given value.
## Fields

```c#
static readonly Vector3 Backward
```
A vector with X set to -1. This represents the backwards direction.
```c#
static readonly Vector3 Down
```
A vector with Z set to -1. This represents the downwards direction.
```c#
static readonly Vector3 Forward
```
A vector with X set to 1. This represents the forwards direction.
```c#
static readonly Vector3 Left
```
A vector with Y set to 1. This represents the left hand direction.
```c#
static readonly Vector3 One
```
A vector with all components set to 1.
```c#
static readonly Vector3 Right
```
A vector with Y set to -1. This represents the right hand direction.
```c#
static readonly Vector3 Up
```
A vector with Z set to 1. This represents the upwards direction.
```c#
static readonly Vector3 Zero
```
A vector with all components set to 0.
## Properties

```c#
static Vector3 Random { get; } 
```
Uniformly samples a 3D position from all points with distance at most 1 from the origin.
```c#
Angles EulerAngles { get; set; } 
```
The Euler angles of this direction vector.
```c#
bool IsNaN { get; } 
```
Returns true if x, y or z are NaN
```c#
bool IsNearZeroLength { get; } 
```
Whether length of this vector is nearly zero.
```c#
float Length { get; } 
```
Length (or magnitude) of the vector (Distance from 0,0,0).
```c#
float LengthSquared { get; } 
```
Squared length of the vector. This is faster thanLength, and can be used for things like comparing distances, as long as only squared values are used.
```c#
Vector3 Normal { get; } 
```
Returns a unit version of this vector. A unit vector has length of 1.
```c#
float x { get; set; } 
```
The X component of this Vector.
```c#
float y { get; set; } 
```
The Y component of this Vector.
```c#
float z { get; set; } 
```
The Z component of this Vector.
## Methods

```c#
static Vector3 Cross( Vector3 a, Vector3 b) 
```
Returns the cross product of the 2 given vectors.
If the given vectors are linearly independent, the resulting vector is perpendicular to them both, also known as a normal of a plane.
```c#
static Vector3 CubicBeizer( Vector3 source, Vector3 target, Vector3 sourceTangent, Vector3 targetTangent, float t) 
```
Calculates position of a point on a cubic beizer curve at given fraction.
```c#
static float DistanceBetween( Vector3 a, Vector3 b) 
```
Returns distance between the 2 given vectors.
```c#
static float DistanceBetweenSquared( Vector3 a, Vector3 b) 
```
Returns squared distance between the 2 given vectors. This is faster thanDistanceBetween,
and can be used for things like comparing distances, as long as only squared values are used.
```c#
static float Dot( Vector3 a, Vector3 b) 
```
Returns the scalar/dot product of the 2 given vectors.
```c#
static float GetAngle( Vector3 v1, Vector3 v2) 
```
Return the distance between the two direction vectors in degrees.
```c#
static Vector3 Lerp( Vector3 a, Vector3 b, float frac, bool clamp = true) 
```
Performs linear interpolation between 2 given vectors.
```c#
static Vector3 Lerp( Vector3 a, Vector3 b, Vector3 frac, bool clamp = true) 
```
Performs linear interpolation between 2 given vectors, with separate fraction for each vector component.
```c#
static Vector3 Max( Vector3 a, Vector3 b) 
```
Returns a vector that has the maximum values on each axis between the 2 given vectors.
```c#
static Vector3 Min( Vector3 a, Vector3 b) 
```
Returns a vector that has the minimum values on each axis between the 2 given vectors.
```c#
static Vector3 Parse( string str, IFormatProvider provider) 
```
ImplementsIParsable`1.Parse
```c#
static Vector3 Parse( string str) 
```
No Summary
```c#
static Vector3 Read( BinaryReader reader) 
```
Read a vector3 from given binary reader.
```c#
static Vector3 Reflect( Vector3 direction, Vector3 normal) 
```
Returns a reflected vector based on incoming direction and plane normal. Like a ray reflecting off of a mirror.
```c#
static Vector3 SmoothDamp( Vector3 current, Vector3 target, ref Vector3 velocity, float smoothTime, float deltaTime) 
```
Smoothly move towards the target vector
```c#
static void Sort( ref Vector3 min, ref Vector3 max) 
```
Sort these two vectors into min and max. This doesn't just swap the vectors, it sorts each component.
So that min will come out containing the minimum x, y and z values.
```c#
static bool TryParse( string str, out Vector3 result) 
```
No Summary
```c#
static bool TryParse( string str, IFormatProvider provider, out Vector3 result) 
```
ImplementsIParsable`1.TryParseGiven a string, try to convert this into a vector. Example input formats that work would be "1,1,1", "1;1;1", "[1 1 1]".This handles a bunch of different separators ( ' ', ',', ';', '\n', '\r' ).It also trims surrounding characters ('[', ']', ' ', '\n', '\r', '\t', '"').
```c#
static Angles VectorAngle( Vector3 vec) 
```
Converts a direction vector to an angle.
```c#
static Vector3 VectorPlaneProject( Vector3 v, Vector3 planeNormal) 
```
Projects given vectoron a plane defined byplaneNormal.
```c#
Vector3 Abs( ) 
```
Returns a new vector with all values positive. -5 becomes 5, etc.
```c#
Vector3 AddClamped( Vector3 toAdd, float maxLength) 
```
Try to add to this vector. If we're already over max then don't add.
If we're over max when we add, clamp in that direction so we're not.
```c#
bool AlmostEqual( Vector3 v, float delta = 0.0001) 
```
Returns true if we're nearly equal to the passed vector.
```c#
float Angle( Vector3 v2) 
```
Return the distance between the two direction vectors in degrees.
```c#
Vector3 Approach( float length, float amount) 
```
Returns a new vector whose length is closer to given target length by given amount.
```c#
Vector3 Clamp( Vector3 otherMin, Vector3 otherMax) 
```
Returns a vector each axis of which is clamped to between the 2 given vectors. Basically clamps a point to an Axis Aligned Bounding Box (AABB).
```c#
Vector3 Clamp( float min, float max) 
```
Returns a vector each axis of which is clamped to given min and max values.
```c#
Vector3 ClampLength( float maxLength) 
```
Returns a vector whose length is limited to given maximum.
```c#
Vector3 ClampLength( float minLength, float maxLength) 
```
Returns a vector whose length is limited between given minimum and maximum.
```c#
Vector3 ComponentMax( Vector3 other) 
```
Returns a vector that has the maximum values on each axis between this vector and given vector.
```c#
Vector3 ComponentMin( Vector3 other) 
```
Returns a vector that has the minimum values on each axis between this vector and given vector.
```c#
Vector3 Cross( Vector3 b) 
```
Returns the cross product of this and the given vector.
If this and the given vectors are linearly independent, the resulting vector is perpendicular to them both, also known as a normal of a plane.
```c#
float Distance( Vector3 target) 
```
Returns distance between this vector to given vector.
```c#
float DistanceSquared( Vector3 target) 
```
Returns squared distance between this vector to given vector. This is faster thanDistance,
and can be used for things like comparing distances, as long as only squared values are used.
```c#
float Dot( Vector3 b) 
```
Returns the scalar/dot product of this and the given vectors.
```c#
bool IsNearlyZero( float tolerance = 1E-45) 
```
Returns true if value on every axis is less than tolerance away from zero
```c#
Vector3 LerpTo( Vector3 target, float frac, bool clamp = true) 
```
Performs linear interpolation between this and given vectors.
```c#
Vector3 LerpTo( Vector3 target, Vector3 frac, bool clamp = true) 
```
Performs linear interpolation between this and given vectors, with separate fraction for each vector component.
```c#
Vector3 ProjectOnNormal( Vector3 normal) 
```
Projects this vectoronto another vector.Basically extends the given normal/unit vector to be as long as necessary to make a right triangle (a triangle which has a 90 degree corner)
between (0,0,0), this vector and the projected vector.
```c#
Vector3 RotateAround( Vector3 center, Rotation rot) 
```
Rotate this vector around given point by given rotation and return the result as a new vector.SeeTransform.RotateAroundfor similar method that also transforms rotation.
```c#
Vector3 SnapToGrid( float gridSize, bool sx = true, bool sy = true, bool sz = true) 
```
Snap to grid along any of the 3 axes.
```c#
Vector3 SubtractDirection( Vector3 direction, float strength = 1) 
```
Given a vector like 1,1,1 and direction 1,0,0, will return 0,1,1.
This is useful for velocity collision type events, where you want to
cancel out velocity based on a normal.
For this to work properly, direction should be a normal, but you can scale
how much you want to subtract by scaling the direction. Ie, passing in a direction
with a length of 0.5 will remove half the direction.
```c#
Vector3 WithX( float x) 
```
Returns this vector with given X component.
```c#
Vector3 WithY( float y) 
```
Returns this vector with given Y component.
```c#
Vector3 WithZ( float z) 
```
Returns this vector with given Z component.
```c#
void Write( BinaryWriter writer) 
```
Write this vector3 to a System.IO.BinaryWriter.
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( Vector3 o) 
```
OverridesValueType.Equals
```c#
override int GetHashCode( ) 
```
OverridesValueType.GetHashCode
```c#
override string ToString( ) 
```
OverridesValueType.ToStringFormats the Vector into a string "x,y,z"
## Extensions

```c#
Vector3 ToScreen( ) 
```
Clientside, returns position of this 3D vector on local clients' screen in 2D coordinates based on theSandbox.Camera.
```c#
Vector2? ToScreen( Vector2 screenSize) 
```
Same asSandboxGameExtensions.ToScreen, but return value is in absolute coordinates.
## Operators

```c#
float this[ int index, ] 
```
No Summary
```c#
Vector3 +( Vector3 c1, Vector3 c2) 
```
No Summary
```c#
Vector3 /( Vector3 c1, float f) 
```
No Summary
```c#
bool ==( Vector3 left, Vector3 right) 
```
No Summary
```c#
bool !=( Vector3 left, Vector3 right) 
```
No Summary
```c#
Vector3 *( Vector3 c1, float f) 
```
No Summary
```c#
Vector3 *( Vector3 c1, Rotation f) 
```
No Summary
```c#
Vector3 *( Vector3 c1, Vector3 c2) 
```
No Summary
```c#
Vector3 *( float f, Vector3 c1) 
```
No Summary
```c#
Vector3 -( Vector3 c1, Vector3 c2) 
```
No Summary
```c#
Vector3 -( Vector3 value) 
```
No Summary
```c#
implicit Vector3 =( Color value) 
```
No Summary
```c#
implicit Vector3 =( float value) 
```
No Summary
```c#
implicit Vector3 =( Vector2 value) 
```
No Summary
```c#
implicit Vector3 =( Vector4 vec) 
```
No Summary
```c#
implicit Vector3 =( Vector3 value) 
```
No Summary
```c#
implicit Vector3 =( Vector3 value) 
```
No Summary
## Referencing Members

```c#
Vector3 = Line.a
```
```c#
Vector3 = Triangle.A
```
```c#
Vector3 = AudioMaterial.Absorption { get; set; } 
```
```c#
virtual void WalkController.Accelerate( Vector3, float, float, float ) 
```
```c#
Transform = Transform.Add( Vector3, bool ) 
```
```c#
static void SandboxBaseExtensions.Add( VertexBuffer, Vector3 ) 
```
```c#
static void SandboxBaseExtensions.Add( VertexBuffer, Vector3, Vector2 ) 
```
```c#
void PhysicsGroup.AddAngularVelocity( Vector3 ) 
```
```c#
ModelBuilder = ModelBuilder.AddBone( string, Vector3, Rotation, string ) 
```
```c#
PhysicsShape = PhysicsBody.AddBoxShape( Vector3, Rotation, Vector3, bool ) 
```
```c#
PhysicsShape = PhysicsBody.AddCapsuleShape( Vector3, Vector3, float, bool ) 
```
```c#
ModelBuilder = ModelBuilder.AddCollisionBox( Vector3, Vector3?, Rotation? ) 
```
```c#
ModelBuilder = ModelBuilder.AddCollisionCapsule( Vector3, Vector3, float ) 
```
```c#
ModelBuilder = ModelBuilder.AddCollisionHull( Vector3[], Vector3?, Rotation? ) 
```
```c#
ModelBuilder = ModelBuilder.AddCollisionSphere( float, Vector3 ) 
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
PhysicsShape = PhysicsBody.AddMeshShape( List<Vector3>, List<int> ) 
```
```c#
PhysicsShape = PhysicsBody.AddMeshShape( Span<Vector3>, Span<int> ) 
```
```c#
BBox = BBox.AddPoint( Vector3 ) 
```
```c#
static void SandboxBaseExtensions.AddQuad( VertexBuffer, Vector3, Vector3, Vector3, Vector3 ) 
```
```c#
static void SandboxBaseExtensions.AddQuad( VertexBuffer, Ray, Vector3, Vector3 ) 
```
```c#
bool = PanelTransform.AddRotation( Vector3 ) 
```
```c#
bool = PanelTransform.AddScale( Vector3 ) 
```
```c#
PhysicsShape = PhysicsBody.AddSphereShape( Vector3, float, bool ) 
```
```c#
NavPathBuilder = NavPathBuilder.AddStop( Vector3 ) 
```
```c#
void PhysicsGroup.AddVelocity( Vector3 ) 
```
```c#
int = PolygonMesh.AddVertex( Vector3 ) 
```
```c#
static Vector3 = Input.AnalogMove { get; set; } 
```
```c#
Angles.Angles( Vector3 ) 
```
```c#
static Vector3 = Angles.AngleVector( Angles ) 
```
```c#
Vector3 = PhysicsBody.AngularVelocity { get; set; } 
```
```c#
Vector3 = PhysicsGroup.AngularVelocity { set; } 
```
```c#
Vector3 = InputMotionData.AngularVelocity
```
```c#
void Entity.ApplyAbsoluteImpulse( Vector3 ) 
```
```c#
void PhysicsBody.ApplyAngularImpulse( Vector3 ) 
```
```c#
void PhysicsGroup.ApplyAngularImpulse( Vector3, bool ) 
```
```c#
void PhysicsBody.ApplyForce( Vector3 ) 
```
```c#
void PhysicsBody.ApplyForceAt( Vector3, Vector3 ) 
```
```c#
void PhysicsBody.ApplyImpulse( Vector3 ) 
```
```c#
void PhysicsGroup.ApplyImpulse( Vector3, bool ) 
```
```c#
void PhysicsBody.ApplyImpulseAt( Vector3, Vector3 ) 
```
```c#
void Entity.ApplyLocalAngularImpulse( Vector3 ) 
```
```c#
void Entity.ApplyLocalImpulse( Vector3 ) 
```
```c#
void PhysicsBody.ApplyTorque( Vector3 ) 
```
```c#
bool = GizmoControls.Arrow( string, Vector3, out float, float, float, float, float, float, string ) 
```
```c#
Vector3 = Angles.AsVector3( ) 
```
```c#
Vector3 = ModelParticle.AttachmentOffset { get; set; } 
```
```c#
Vector3 = LengthConstraint.AttachPoint { get; set; } 
```
```c#
void DebugOverlay.Axis( Vector3, Rotation, float, float, bool ) 
```
```c#
Vector3 = Line.b
```
```c#
Vector3 = Triangle.B
```
```c#
Vector3 = Rotation.Backward { get; } 
```
```c#
Vector3 = Transform.Backward { get; } 
```
```c#
Vector3 = Entity.BaseVelocity { get; set; } 
```
```c#
Vector3 = PawnController.BaseVelocity { get; set; } 
```
```c#
BBox.BBox( Vector3, Vector3 ) 
```
```c#
BBox.BBox( Vector3, float ) 
```
```c#
Bone.Bone( string, string, Vector3, Rotation ) 
```
```c#
PhysicsTraceBuilder = PhysicsTraceBuilder.Box( Vector3, in Vector3, in Vector3 ) 
```
```c#
PhysicsTraceBuilder = PhysicsTraceBuilder.Box( Vector3, in Ray, in float ) 
```
```c#
static Trace = Trace.Box( Vector3, in Vector3, in Vector3 ) 
```
```c#
static Trace = Trace.Box( Vector3, in Ray, in float ) 
```
```c#
void DebugOverlay.Box( Vector3, Vector3 ) 
```
```c#
void DebugOverlay.Box( Vector3, Vector3, Color, float, bool ) 
```
```c#
void DebugOverlay.Box( Vector3, Vector3, Vector3, Color, float, bool ) 
```
```c#
void DebugOverlay.Box( Vector3, Rotation, Vector3, Vector3, Color, float, bool ) 
```
```c#
Vector3 = VisibilityBoxEntity.BoxSize { get; set; } 
```
```c#
static void Breakables.Break( Model, Vector3, Rotation, float, Color, Result, PhysicsBody ) 
```
```c#
void VoxelChunk.BreakWorldSpace( Vector3 ) 
```
```c#
NavPath = NavPathBuilder.Build( Vector3 ) 
```
```c#
static Vector3[] = NavMesh.BuildPath( Vector3, Vector3 ) 
```
```c#
static bool = NavMesh.BuildPath( Vector3, Vector3, List<Vector3> ) 
```
```c#
Vector3 = Triangle.C
```
```c#
Capsule.Capsule( Vector3, Vector3, float ) 
```
```c#
Vector3 = BBox.Center { get; } 
```
```c#
Vector3 = Line.Center { get; } 
```
```c#
Vector3 = Sphere.Center { get; set; } 
```
```c#
Vector3 = Node.Center { get; } 
```
```c#
Vector3 = NavArea.Center { get; } 
```
```c#
Vector3 = ModelSphereAOProxy.Center { get; set; } 
```
```c#
Vector3 = Capsule.CenterA
```
```c#
Vector3 = Capsule.CenterB
```
```c#
void GizmoHitbox.Circle( Vector3, Vector3, float, float ) 
```
```c#
void DebugOverlay.Circle( Vector3, Rotation, float, Color, float, bool ) 
```
```c#
Vector3 = BBox.ClosestPoint( Vector3 ) 
```
```c#
Vector3 = BBox.ClosestPoint( Vector3 ) 
```
```c#
Vector3 = Line.ClosestPoint( in Vector3 ) 
```
```c#
Vector3 = Triangle.ClosestPoint( in Vector3 ) 
```
```c#
Vector3 = Node.ClosestPoint( Vector3 ) 
```
```c#
Vector3 = Node.ClosestPoint( Vector3 ) 
```
```c#
Vector3 = ModelEntity.CollisionPosition { get; } 
```
```c#
Vector3 = ModelEntity.CollisionWorldSpaceCenter { get; } 
```
```c#
bool = BBox.Contains( Vector3 ) 
```
```c#
static void SandboxBaseExtensions.CopyBonesFrom( Entity, Entity, Vector3, Rotation, float ) 
```
```c#
IEnumerable<Vector3> = BBox.Corners { get; } 
```
```c#
static Particles = Particles.Create( string, Vector3 ) 
```
```c#
static NavPathBuilder = NavPathBuilder.Create( Vector3 ) 
```
```c#
static BallSocketJoint = PhysicsJoint.CreateBallSocket( PhysicsBody, PhysicsBody, Vector3 ) 
```
```c#
static HingeJoint = PhysicsJoint.CreateHinge( PhysicsBody, PhysicsBody, Vector3, Vector3 ) 
```
```c#
static PulleyJoint = PhysicsJoint.CreatePulley( PhysicsBody, PhysicsBody, Vector3, Vector3, Vector3, Vector3 ) 
```
```c#
static Matrix = Matrix.CreateRotation( Vector3 ) 
```
```c#
static Matrix = Matrix.CreateRotationX( float, Vector3 ) 
```
```c#
static Matrix = Matrix.CreateRotationY( float, Vector3 ) 
```
```c#
static Matrix = Matrix.CreateRotationZ( float, Vector3 ) 
```
```c#
static Matrix = Matrix.CreateScale( Vector3 ) 
```
```c#
static Matrix = Matrix.CreateScale( Vector3, Vector3 ) 
```
```c#
static SliderJoint = PhysicsJoint.CreateSlider( PhysicsBody, PhysicsBody, Vector3, float, float ) 
```
```c#
static Matrix = Matrix.CreateTranslation( Vector3 ) 
```
```c#
static Matrix = Matrix.CreateWorld( Vector3, Vector3, Vector3 ) 
```
```c#
Vector3 = BreakableParams.DamagePositon
```
```c#
Vector3 = Entry.Data
```
```c#
Vector3 = ParticleSystemEntity.DataControlPointValue { get; set; } 
```
```c#
Vector3 = Line.Delta { get; } 
```
```c#
Vector3 = ModelBoxAOProxy.Dimensions { get; set; } 
```
```c#
Vector3 = ModelEyeOcclusion.Dimensions { get; set; } 
```
```c#
Vector3 = PhysicsTraceResult.Direction
```
```c#
Vector3 = TraceResult.Direction
```
```c#
float = Line.Distance( Vector3 ) 
```
```c#
float = Line.Distance( Vector3, out Vector3 ) 
```
```c#
float = Node.Distance( Vector3 ) 
```
```c#
Vector3 = Rotation.Down { get; } 
```
```c#
Vector3 = Transform.Down { get; } 
```
```c#
static void ToolRender.DrawBox( Vector3, Vector3, Color ) 
```
```c#
static void ToolRender.DrawLine( Vector3, Vector3, Color, Color ) 
```
```c#
static void ToolRender.DrawLine( Vector3, Vector3, Color ) 
```
```c#
static void ToolRender.DrawWorldSpaceText( string, Vector3, Vector2, Color, float ) 
```
```c#
Vector3 = Line.End { get; } 
```
```c#
Vector3 = NavigationPath.EndPoint { get; set; } 
```
```c#
Vector3 = PhysicsTraceResult.EndPosition
```
```c#
Vector3 = Result.EndPosition { get; set; } 
```
```c#
Vector3 = TraceResult.EndPosition
```
```c#
Vector3 = SoundscapeBoxEntity.Extents { get; set; } 
```
```c#
Vector3 = PawnController.EyeLocalPosition { get; set; } 
```
```c#
Vector3 = Player.EyeLocalPosition { get; set; } 
```
```c#
Vector3 = Player.EyePosition { get; set; } 
```
```c#
Vector3 = ShatterGlass.FaceAxisForward { get; set; } 
```
```c#
Vector3 = VoxelSurface.FaceAxisForward { get; set; } 
```
```c#
Vector3 = ShatterGlass.FaceAxisRight { get; set; } 
```
```c#
Vector3 = VoxelSurface.FaceAxisRight { get; set; } 
```
```c#
Vector3 = ShatterGlass.FaceCenter { get; set; } 
```
```c#
Vector3 = VoxelSurface.FaceCenter { get; set; } 
```
```c#
static Vector3 = Noise.FbmVector( int, float, float ) 
```
```c#
Vector3 = PhysicsBody.FindClosestPoint( Vector3 ) 
```
```c#
Vector3 = PhysicsBody.FindClosestPoint( Vector3 ) 
```
```c#
static IEnumerable<Entity> = Entity.FindInSphere( Vector3, float ) 
```
```c#
Vector3 = NavArea.FindRandomConnectedPoint( Vector3, NavAgentHull, float, float ) 
```
```c#
Vector3 = NavArea.FindRandomConnectedPoint( Vector3, NavAgentHull, float, float ) 
```
```c#
Vector3 = NavArea.FindRandomSpot( ) 
```
```c#
Vector3 = DamageInfo.Force { get; set; } 
```
```c#
Vector3 = Angles.Forward { get; set; } 
```
```c#
Vector3 = Ray.Forward { get; set; } 
```
```c#
Vector3 = Rotation.Forward { get; } 
```
```c#
Vector3 = Transform.Forward { get; } 
```
```c#
Vector3 = NavPathSegment.Forward { get; } 
```
```c#
static Rotation = Rotation.FromAxis( Vector3, float ) 
```
```c#
static DamageInfo = DamageInfo.FromBullet( Vector3, Vector3, float ) 
```
```c#
static DamageInfo = DamageInfo.FromExplosion( Vector3, Vector3, float ) 
```
```c#
static BBox = BBox.FromPoints( IEnumerable<Vector3>, float ) 
```
```c#
static BBox = BBox.FromPositionAndSize( Vector3, float ) 
```
```c#
static BBox = BBox.FromPositionAndSize( Vector3, Vector3 ) 
```
```c#
static Sound = Sound.FromWorld( To, string, Vector3 ) 
```
```c#
static Sound = Sound.FromWorld( string, Vector3 ) 
```
```c#
static Vector3 = SandboxSystemExtensions.Gaussian3D( Random, Vector3?, Vector3? ) 
```
```c#
static Vector3 = SandboxSystemExtensions.Gaussian3D( Random, Vector3?, Vector3? ) 
```
```c#
GenericEvent.GenericEvent( string, int, float, string, Vector3 ) 
```
```c#
Vector3 = AnimatedEntity.GetAnimParameterVector( string ) 
```
```c#
static NavAreaAttribute = NavMesh.GetAreaAttribute( Vector3 ) 
```
```c#
static NavArea = NavArea.GetClosestNav( Vector3, NavAgentHull, GetNavAreaFlags, ref Vector3, float, float, float, float ) 
```
```c#
static NavArea = NavArea.GetClosestNav( Vector3, NavAgentHull, GetNavAreaFlags, float, float, float, float ) 
```
```c#
static Vector3? = NavMesh.GetClosestPoint( Vector3 ) 
```
```c#
static Vector3? = NavMesh.GetClosestPoint( Vector3 ) 
```
```c#
Vector3 = SceneParticles.GetControlPointPosition( int ) 
```
```c#
Vector3? = Frustum.GetCorner( int ) 
```
```c#
static Vector3 = Gizmo.GetCursorDelta( ) 
```
```c#
static Vector3 = Screen.GetDirection( Vector2 ) 
```
```c#
static Vector3 = Screen.GetDirection( Vector2, float ) 
```
```c#
static Vector3 = Screen.GetDirection( Vector2, float, Rotation ) 
```
```c#
static Vector3 = Screen.GetDirection( Vector2, float, Rotation, Vector2 ) 
```
```c#
float = Plane.GetDistance( Vector3 ) 
```
```c#
static Vector3? = Plane.GetIntersection( Plane, Plane, Plane ) 
```
```c#
static Vector3 = Gizmo.GetMouseDelta( Vector3, Vector3 ) 
```
```c#
static Vector3 = Gizmo.GetMouseDelta( Vector3, Vector3 ) 
```
```c#
static float = Gizmo.GetMouseDistance( Vector3, Vector3 ) 
```
```c#
static float = Gizmo.GetMouseDistanceDelta( Vector3, Vector3 ) 
```
```c#
Vector3 = BasePathEntity<T>.GetPointBetweenNodes( IBasePathNode, IBasePathNode, float, bool ) 
```
```c#
static Vector3? = NavMesh.GetPointWithinRadius( Vector3, float, float ) 
```
```c#
static Vector3? = NavMesh.GetPointWithinRadius( Vector3, float, float ) 
```
```c#
Vector3 = NavigationPath.GetPositionAlongPath( float ) 
```
```c#
static Vector3? = Gizmo.GetPositionOnPlane( Vector3, Vector3, Ray ) 
```
```c#
static Vector3? = Gizmo.GetPositionOnPlane( Vector3, Vector3, Ray ) 
```
```c#
Ray = SceneCamera.GetRay( Vector3 ) 
```
```c#
Ray = SceneCamera.GetRay( Vector3, Vector3 ) 
```
```c#
Vector3 = RenderAttributes.GetVector( in string, in Vector3 ) 
```
```c#
Vector3 = SceneModel.GetVector3( string ) 
```
```c#
Vector3 = PhysicsBody.GetVelocityAtPoint( Vector3 ) 
```
```c#
Vector3 = PhysicsBody.GetVelocityAtPoint( Vector3 ) 
```
```c#
Vector3 = PhysicsWorld.Gravity { get; set; } 
```
```c#
Vector3 = PhysicsSettings.Gravity { get; set; } 
```
```c#
Vector3 = PawnController.GroundNormal { get; set; } 
```
```c#
Vector3 = HingeConstraint.HingeAxis { get; set; } 
```
```c#
Vector3 = Result.HitNormal { get; set; } 
```
```c#
Vector3 = PhysicsTraceResult.HitPosition
```
```c#
Vector3 = Result.HitPosition { get; set; } 
```
```c#
Vector3 = TraceResult.HitPosition
```
```c#
Vector3 = TraceResult.HitPosition
```
```c#
Vector3 = PhysicsBody.Inertia { get; } 
```
```c#
Vector3 = Player.InputDirection { get; protected set; } 
```
```c#
bool = Plane.IsInFront( Vector3 ) 
```
```c#
bool = Frustum.IsInside( Vector3 ) 
```
```c#
Vector3 = Rotation.Left { get; } 
```
```c#
Vector3 = Transform.Left { get; } 
```
```c#
Vector3 = SkyLightInfo.LightColor
```
```c#
Vector3 = SkyLightInfo.LightDirection
```
```c#
Line.Line( Vector3, Vector3 ) 
```
```c#
Line.Line( Vector3, Vector3, float ) 
```
```c#
void DebugOverlay.Line( Vector3, Vector3, Color, float, bool ) 
```
```c#
void DebugOverlay.Line( Vector3, Vector3, float, bool ) 
```
```c#
void GizmoDraw.LineCylinder( Vector3, Vector3, float, float, int ) 
```
```c#
static PhysicsPoint = PhysicsPoint.Local( PhysicsBody, Vector3?, Rotation? ) 
```
```c#
Task<bool> = KeyframeEntity.LocalKeyframeTo( Vector3, float, Function ) 
```
```c#
Vector3 = PhysicsBody.LocalMassCenter { get; set; } 
```
```c#
PhysicsPoint = PhysicsBody.LocalPoint( Vector3 ) 
```
```c#
Vector3 = PhysicsPoint.LocalPosition
```
```c#
virtual Vector3 = Entity.LocalPosition { get; set; } 
```
```c#
override Vector3 = ModelEntity.LocalPosition { get; set; } 
```
```c#
virtual Vector3 = Entity.LocalVelocity { get; set; } 
```
```c#
static Rotation = Rotation.LookAt( Vector3, Vector3 ) 
```
```c#
static Rotation = Rotation.LookAt( Vector3 ) 
```
```c#
Vector3 = PhysicsBody.MassCenter { get; } 
```
```c#
Vector3 = PhysicsGroup.MassCenter { get; } 
```
```c#
protected Vector3 = WalkController.maxs
```
```c#
Vector3 = BBox.Maxs
```
```c#
protected Vector3 = WalkController.mins
```
```c#
Vector3 = BBox.Mins
```
```c#
void FlyingController.Move( Vector3, int ) 
```
```c#
MoveHelper.MoveHelper( Vector3, Vector3, string[] ) 
```
```c#
MoveHelper.MoveHelper( Vector3, Vector3 ) 
```
```c#
Vector3 = ParticleSystemEntity.NamedVectorValue { get; set; } 
```
```c#
NavPathBuilder.NavPathBuilder( Vector3 ) 
```
```c#
Vector3 = SimpleVertex.normal
```
```c#
Vector3 = Plane.Normal
```
```c#
Vector3 = Triangle.Normal { get; } 
```
```c#
Vector3 = PhysicsTraceResult.Normal
```
```c#
readonly Vector3 = PhysicsContact.Normal
```
```c#
Vector3 = Vertex.Normal
```
```c#
Vector3 = Node.Normal { get; } 
```
```c#
Vector3 = Vertex.Normal
```
```c#
Vector3 = VertexDetail.Normal { get; set; } 
```
```c#
Vector3 = CollisionEventData.Normal
```
```c#
Vector3 = NavArea.Normal { get; } 
```
```c#
Vector3 = TraceResult.Normal
```
```c#
Vector3 = TraceResult.Normal
```
```c#
Vector3 = Transform.NormalToLocal( Vector3 ) 
```
```c#
Vector3 = Transform.NormalToLocal( Vector3 ) 
```
```c#
Vector3 = Transform.NormalToWorld( Vector3 ) 
```
```c#
Vector3 = Transform.NormalToWorld( Vector3 ) 
```
```c#
Vector3 = SkyboxAccessor.Offset { get; set; } 
```
```c#
Vector3 = ModelBreakPiece.Offset { get; set; } 
```
```c#
Vector3 = ChromaticAberrationSettings.Offset { get; set; } 
```
```c#
virtual void ModelEntity.OnAnimEventFootstep( Vector3, int, float ) 
```
```c#
override void Player.OnAnimEventFootstep( Vector3, int, float ) 
```
```c#
virtual void ModelEntity.OnAnimEventGeneric( string, int, float, Vector3, string ) 
```
```c#
protected virtual void AnimatedEntity.OnAnimFootstep( bool, Vector3 ) 
```
```c#
static Angles = Angles.op_Addition( Angles, Vector3 ) 
```
```c#
static BBox = BBox.op_Addition( BBox, Vector3 ) 
```
```c#
static Color = Color.op_Implicit( Vector3 ) 
```
```c#
static Vector2 = Vector2.op_Implicit( Vector3 ) 
```
```c#
static Vector3 = PhysicsSpring.op_Implicit( PhysicsSpring ) 
```
```c#
static PhysicsSpring = PhysicsSpring.op_Implicit( Vector3 ) 
```
```c#
static Vector3 = Rotation.op_Multiply( Rotation, Vector3 ) 
```
```c#
static Vector3 = Rotation.op_Multiply( Rotation, Vector3 ) 
```
```c#
Vector3 = Plane.Origin { get; } 
```
```c#
Vector3 = ModelBoxAOProxy.OriginOffset { get; set; } 
```
```c#
Vector3 = ModelEyeOcclusion.OriginOffset { get; set; } 
```
```c#
static NavPathBuilder = NavMesh.PathBuilder( Vector3 ) 
```
```c#
PhysicsPoint.PhysicsPoint( PhysicsBody, Vector3?, Rotation? ) 
```
```c#
static Vector3 = Selection.PivotPosition { get; set; } 
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
Plane.Plane( Vector3, double ) 
```
```c#
Plane.Plane( Vector3, Vector3 ) 
```
```c#
Plane.Plane( Vector3, Vector3, Vector3 ) 
```
```c#
void GizmoDraw.Plane( Vector3, Vector3 ) 
```
```c#
abstract void AnimGraphDirectPlayback.Play( string, Vector3, float, float ) 
```
```c#
readonly Vector3 = PhysicsContact.Point
```
```c#
Vector3 = ModelCapsuleAOProxy.Point0 { get; set; } 
```
```c#
Vector3 = ModelCylinderAOProxy.Point0 { get; set; } 
```
```c#
Vector3 = ModelCapsuleAOProxy.Point1 { get; set; } 
```
```c#
Vector3 = ModelCylinderAOProxy.Point1 { get; set; } 
```
```c#
Vector3 = Transform.PointToLocal( Vector3 ) 
```
```c#
Vector3 = Transform.PointToLocal( Vector3 ) 
```
```c#
Vector3 = Transform.PointToWorld( Vector3 ) 
```
```c#
Vector3 = Transform.PointToWorld( Vector3 ) 
```
```c#
Vector3 = PhysicsGroup.Pos { get; } 
```
```c#
Vector3 = SimpleVertex.position
```
```c#
Vector3 = Ray.Position { get; set; } 
```
```c#
Vector3 = Transform.Position
```
```c#
Vector3 = SoundHandle.Position { set; } 
```
```c#
static Vector3 = Camera.Position { get; set; } 
```
```c#
abstract Vector3 = IEntity.Position { get; set; } 
```
```c#
Vector3 = PhysicsBody.Position { get; set; } 
```
```c#
Vector3 = Vertex.Position
```
```c#
Vector3 = SceneCamera.Position { get; set; } 
```
```c#
Vector3 = SceneObject.Position { get; set; } 
```
```c#
Vector3 = MusicPlayer.Position { get; set; } 
```
```c#
Vector3 = Segment.Position
```
```c#
bool = GizmoControls.Position( string, Vector3, out Vector3, Rotation?, float ) 
```
```c#
Vector3 = Bone.Position { get; init; } 
```
```c#
Vector3 = Vertex.Position
```
```c#
Vector3 = SkyboxAccessor.Position { get; set; } 
```
```c#
Vector3 = SoundEvent.Position { get; set; } 
```
```c#
abstract Vector3 = EntityObject.Position { get; set; } 
```
```c#
Vector3 = VertexDetail.Position { get; set; } 
```
```c#
virtual Vector3 = Entity.Position { get; set; } 
```
```c#
Vector3 = CollisionEventData.Position
```
```c#
override Vector3 = ModelEntity.Position { get; set; } 
```
```c#
Vector3 = DamageInfo.Position { get; set; } 
```
```c#
Vector3 = NavPathSegment.Position { get; } 
```
```c#
Vector3 = MapNode.Position { get; set; } 
```
```c#
Vector3 = MeshVertex.Position
```
```c#
Vector3 = BasePathNode.Position { get; set; } 
```
```c#
abstract Vector3 = ISoundscapeEntity.Position { get; } 
```
```c#
Vector3 = MoveHelper.Position
```
```c#
Vector3 = PawnController.Position { get; set; } 
```
```c#
Vector3 = WorldPanel.Position { get; set; } 
```
```c#
Vector3 = SplashInformation.Position
```
```c#
Vector3 = PulleyConstraint.Position2 { get; set; } 
```
```c#
Vector3 = InputMotionData.PositionalAcceleration
```
```c#
Vector3 = CollisionEntityData.PostAngularVelocity
```
```c#
Vector3 = CollisionEntityData.PostVelocity
```
```c#
Vector3 = CollisionEntityData.PreAngularVelocity
```
```c#
Vector3 = CollisionEntityData.PreVelocity
```
```c#
Vector3 = Ray.Project( float ) 
```
```c#
Vector3 = BBox.RandomPointInside { get; } 
```
```c#
Ray.Ray( Vector3, Vector3 ) 
```
```c#
static Vector3 = SandboxSystemExtensions.ReadVector3( BinaryReader ) 
```
```c#
Vector3 = Rotation.Right { get; } 
```
```c#
Vector3 = Transform.Right { get; } 
```
```c#
Vector3 = AnimatedEntity.RootMotion { get; } 
```
```c#
Transform = Transform.RotateAround( Vector3, Rotation ) 
```
```c#
Rotation = Rotation.RotateAroundAxis( Vector3, float ) 
```
```c#
Rotation.Rotation( Vector3, float ) 
```
```c#
Vector3 = PhysicsShape.Scale { get; } 
```
```c#
abstract Vector3 = EntityObject.Scale { get; set; } 
```
```c#
Vector3 = MapNode.Scale { get; set; } 
```
```c#
Vector3 = AssetVideo.SceneCenter
```
```c#
SceneCullingBox.SceneCullingBox( SceneWorld, Transform, Vector3, CullMode ) 
```
```c#
SceneLight.SceneLight( SceneWorld, Vector3, float, Color ) 
```
```c#
static ScenePanel = SceneConstructor.ScenePanel( PanelCreator, SceneWorld, Vector3, Rotation, float, string ) 
```
```c#
Vector3 = AssetVideo.SceneSize
```
```c#
SceneSpotLight.SceneSpotLight( SceneWorld, Vector3, Color ) 
```
```c#
static IDisposable = Gizmo.Scope( string, Vector3 ) 
```
```c#
static IDisposable = Gizmo.Scope( string, Vector3, Rotation, float ) 
```
```c#
protected virtual float = NavigationPath.ScoreFor( in Connection, Vector3 ) 
```
```c#
void GizmoDraw.ScreenBiasedHalfCircle( Vector3, float ) 
```
```c#
Vector3 = NavPathSegment.SegmentAcceleration { get; } 
```
```c#
bool = Material.Set( string, Vector3 ) 
```
```c#
void AnimatedEntity.SetAnimLookAt( string, Vector3, Vector3 ) 
```
```c#
void SceneModel.SetAnimParameter( string, Vector3 ) 
```
```c#
void AnimatedEntity.SetAnimParameter( string, Vector3 ) 
```
```c#
virtual void WalkController.SetBBox( Vector3, Vector3 ) 
```
```c#
void Mesh.SetBounds( Vector3, Vector3 ) 
```
```c#
void SceneParticles.SetControlPoint( int, Vector3 ) 
```
```c#
void MapEntity.SetDefaultBounds( Vector3, Vector3 ) 
```
```c#
void Particles.SetEntity( int, Entity, Vector3, bool ) 
```
```c#
void Particles.SetEntityAttachment( int, Entity, string, Vector3, ParticleAttachment ) 
```
```c#
void Particles.SetForward( int, Vector3 ) 
```
```c#
void Particles.SetPosition( int, Vector3 ) 
```
```c#
Sound = Sound.SetPosition( To, Vector3 ) 
```
```c#
Sound = Sound.SetPosition( Vector3 ) 
```
```c#
void SceneSkyBox.SetSkyLighting( Vector3 ) 
```
```c#
PhysicsGroup = ModelEntity.SetupPhysicsFromAABB( PhysicsMotionType, Vector3, Vector3 ) 
```
```c#
PhysicsGroup = ModelEntity.SetupPhysicsFromOBB( PhysicsMotionType, Vector3, Vector3 ) 
```
```c#
PhysicsGroup = ModelEntity.SetupPhysicsFromSphere( PhysicsMotionType, Vector3, float ) 
```
```c#
void GlassShard.ShatterWorldSpace( Vector3 ) 
```
```c#
SimpleVertex.SimpleVertex( Vector3, Vector3, Vector3, Vector2 ) 
```
```c#
Vector3 = BBox.Size { get; } 
```
```c#
Vector3 = SceneCullingBox.Size { get; set; } 
```
```c#
Vector3 = SlideConstraint.SlideAxis { get; set; } 
```
```c#
Vector3 = Plane.SnapToPlane( Vector3 ) 
```
```c#
Vector3 = Plane.SnapToPlane( Vector3 ) 
```
```c#
void GizmoDraw.SolidCapsule( Vector3, Vector3, float, int, int ) 
```
```c#
void GizmoDraw.SolidCircle( Vector3, float, float, float, int ) 
```
```c#
void GizmoDraw.SolidCone( Vector3, Vector3, float, int? ) 
```
```c#
void GizmoDraw.SolidCylinder( Vector3, Vector3, float, int ) 
```
```c#
void GizmoDraw.SolidRing( Vector3, float, float, float, float, int ) 
```
```c#
void GizmoDraw.SolidSphere( Vector3, float, int, int ) 
```
```c#
SoundEvent.SoundEvent( string, Vector3, string ) 
```
```c#
readonly Vector3 = PhysicsContact.Speed
```
```c#
Sphere.Sphere( Vector3, float ) 
```
```c#
void DebugOverlay.Sphere( Vector3, float, Color, float, bool ) 
```
```c#
Vector3 = SpringConstraint.SpringAxis { get; set; } 
```
```c#
void GizmoDraw.Sprite( Vector3, float, string ) 
```
```c#
void GizmoDraw.Sprite( Vector3, float, Texture ) 
```
```c#
void GizmoDraw.Sprite( Vector3, Vector2, Texture, bool ) 
```
```c#
float = Line.SqrDistance( Vector3 ) 
```
```c#
Vector3 = Line.Start { get; } 
```
```c#
Vector3 = NavigationPath.StartPoint { get; set; } 
```
```c#
Vector3 = PhysicsTraceResult.StartPosition
```
```c#
Vector3 = Result.StartPosition { get; set; } 
```
```c#
Vector3 = TraceResult.StartPosition
```
```c#
Vector3 = GlassShard.StressVelocity { get; set; } 
```
```c#
Vector3 = SimpleVertex.tangent
```
```c#
Vector3 = BasePathNode.TangentIn { get; set; } 
```
```c#
Vector3 = BasePathNodeEntity.TangentIn { get; set; } 
```
```c#
Vector3 = BasePathNode.TangentOut { get; set; } 
```
```c#
Vector3 = BasePathNodeEntity.TangentOut { get; set; } 
```
```c#
static bool = Trace.TestPoint( Vector3, string, float ) 
```
```c#
virtual bool = SoundscapeBoxEntity.TestPosition( Vector3 ) 
```
```c#
virtual bool = SoundscapeRadiusEntity.TestPosition( Vector3 ) 
```
```c#
abstract bool = ISoundscapeEntity.TestPosition( Vector3 ) 
```
```c#
void DebugOverlay.Text( string, Vector3, int, Color, float, float ) 
```
```c#
void DebugOverlay.Text( string, Vector3, Color, float, float ) 
```
```c#
void DebugOverlay.Text( string, Vector3, float, float ) 
```
```c#
Vector2 = SceneCamera.ToScreen( Vector3 ) 
```
```c#
static Vector3 = SandboxGameExtensions.ToScreen( Vector3 ) 
```
```c#
static Vector3 = SandboxGameExtensions.ToScreen( Vector3 ) 
```
```c#
static Vector2? = SandboxGameExtensions.ToScreen( Vector3, Vector2 ) 
```
```c#
Vector3? = Plane.Trace( Ray, bool, double ) 
```
```c#
virtual TraceResult = BasePlayerController.TraceBBox( Vector3, Vector3, Vector3, Vector3, float ) 
```
```c#
virtual TraceResult = BasePlayerController.TraceBBox( Vector3, Vector3, float ) 
```
```c#
override TraceResult = WalkController.TraceBBox( Vector3, Vector3, float ) 
```
```c#
virtual IEnumerable<TraceResult> = BaseWeapon.TraceBullet( Vector3, Vector3, float ) 
```
```c#
TraceResult = MoveHelper.TraceDirection( Vector3 ) 
```
```c#
TraceResult = MoveHelper.TraceFromTo( Vector3, Vector3 ) 
```
```c#
TraceResult = MoveHelper.TraceMove( Vector3 ) 
```
```c#
Vector3 = BasePlayerController.TraceOffset
```
```c#
Vector3 = Matrix.Transform( Vector3 ) 
```
```c#
Vector3 = Matrix.Transform( Vector3 ) 
```
```c#
Transform.Transform( Vector3 ) 
```
```c#
Transform.Transform( Vector3, Rotation, float ) 
```
```c#
Vector3 = Matrix.TransformNormal( Vector3 ) 
```
```c#
Vector3 = Matrix.TransformNormal( Vector3 ) 
```
```c#
Vector3 = GlassShard.TransformPosPanelToWorld( Vector2 ) 
```
```c#
Vector2 = GlassShard.TransformPosWorldToPanel( Vector3 ) 
```
```c#
Vector3 = Transform.TransformVector( Vector3 ) 
```
```c#
Vector3 = Transform.TransformVector( Vector3 ) 
```
```c#
BBox = BBox.Translate( Vector3 ) 
```
```c#
Vector3 = AudioMaterial.Transmission { get; set; } 
```
```c#
Triangle.Triangle( Vector3, Vector3, Vector3 ) 
```
```c#
void GlassShard.TryGenerateShardModel( Vector3, Vector3, bool, bool ) 
```
```c#
virtual bool = KeyframeEntity.TryLocalKeyframeTo( Vector3, float ) 
```
```c#
void GizmoHitbox.TrySetHovered( Vector3 ) 
```
```c#
Vector3 = Rotation.Up { get; } 
```
```c#
Vector3 = Transform.Up { get; } 
```
```c#
void PlanarReflection.Update( Vector3, Vector3, float ) 
```
```c#
void PhysicsShape.UpdateMesh( List<Vector3>, List<int> ) 
```
```c#
void PhysicsShape.UpdateMesh( Span<Vector3>, Span<int> ) 
```
```c#
Vector3 = Vector3Property.Value { get; set; } 
```
```c#
Vector3 = GenericEvent.Vector { get; set; } 
```
```c#
Vector2.Vector2( Vector3 ) 
```
```c#
Vector3 = AsAccessor.Vector3 { get; set; } 
```
```c#
static Vector3 = SandboxSystemExtensions.VectorInCube( Random, float ) 
```
```c#
static Vector3 = SandboxSystemExtensions.VectorInSphere( Random, float ) 
```
```c#
abstract Vector3 = IEntity.Velocity { get; set; } 
```
```c#
Vector3 = PhysicsBody.Velocity { get; set; } 
```
```c#
Vector3 = PhysicsGroup.Velocity { set; } 
```
```c#
virtual Vector3 = Entity.Velocity { get; set; } 
```
```c#
Vector3 = CollisionEventData.Velocity
```
```c#
override Vector3 = ModelEntity.Velocity { get; set; } 
```
```c#
Vector3 = VrHand.Velocity { get; } 
```
```c#
Vector3 = MoveHelper.Velocity
```
```c#
Vector3 = PawnController.Velocity { get; set; } 
```
```c#
Vector3 = SplashInformation.Velocity
```
```c#
Vertex.Vertex( Vector3 ) 
```
```c#
Vertex.Vertex( Vector3, Color32 ) 
```
```c#
Vertex.Vertex( Vector3, Vector4, Color32 ) 
```
```c#
Vertex.Vertex( Vector3, Vector3, Vector3, Vector4 ) 
```
```c#
Vector3 = Result.VertexInfluence { get; set; } 
```
```c#
List<Vector3> = Node.Vertices { get; } 
```
```c#
Vector3 = ScenePortal.ViewPosition { get; set; } 
```
```c#
Vector3 = PawnController.WishVelocity { get; set; } 
```
```c#
DamageInfo = DamageInfo.WithForce( Vector3 ) 
```
```c#
void CitizenAnimationHelper.WithLookAt( Vector3, float, float, float ) 
```
```c#
Transform = Transform.WithPosition( Vector3 ) 
```
```c#
Transform = Transform.WithPosition( Vector3, Rotation ) 
```
```c#
DamageInfo = DamageInfo.WithPosition( Vector3 ) 
```
```c#
Texture3DBuilder = Texture3DBuilder.WithSize( Vector3 ) 
```
```c#
NavPathBuilder = NavPathBuilder.WithStartAcceleration( Vector3 ) 
```
```c#
NavPathBuilder = NavPathBuilder.WithStartVelocity( Vector3 ) 
```
```c#
void CitizenAnimationHelper.WithVelocity( Vector3 ) 
```
```c#
void CitizenAnimationHelper.WithWishVelocity( Vector3 ) 
```
```c#
static PhysicsPoint = PhysicsPoint.World( PhysicsBody, Vector3?, Rotation? ) 
```
```c#
PhysicsPoint = PhysicsBody.WorldPoint( Vector3 ) 
```
```c#
abstract Vector3 = IBasePathNode.WorldPosition { get; } 
```
```c#
virtual Vector3 = BasePathNode.WorldPosition { get; } 
```
```c#
virtual Vector3 = BasePathNodeEntity.WorldPosition { get; } 
```
```c#
abstract Vector3 = IBasePathNode.WorldTangentIn { get; } 
```
```c#
virtual Vector3 = BasePathNode.WorldTangentIn { get; } 
```
```c#
virtual Vector3 = BasePathNodeEntity.WorldTangentIn { get; } 
```
```c#
abstract Vector3 = IBasePathNode.WorldTangentOut { get; } 
```
```c#
virtual Vector3 = BasePathNode.WorldTangentOut { get; } 
```
```c#
virtual Vector3 = BasePathNodeEntity.WorldTangentOut { get; } 
```
```c#
static void SandboxSystemExtensions.Write( BinaryWriter, Vector3 ) 
```
