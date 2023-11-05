# Angles

## ```c#
Implements IEquatable<Angles>, IParsable<Angles>
```

## Summary

Euler angles. Unlike aRotation, Euler angles can represent multiple revolutions (rotations) around an axis,
but suffer from issues likegimbal lockand lack of a defined "up" vector.
## Constructors

```c#
Angles( float pitch, float yaw, float roll) 
```
Initializes the angles object with given components.
```c#
Angles( Angles other) 
```
Copies values of given angles object.
```c#
Angles( Vector3 vector) 
```
Where x, y and z represent the pitch, yaw and roll respectively.
```c#
Angles( float all = 0) 
```
Initializes the angles object with all components set to given value.
## Fields

```c#
static readonly Angles Zero
```
An angle constant that has all its values set to 0. Use this instead of making a static 0,0,0 object yourself.
```c#
float pitch
```
The pitch component, typically up/down.
```c#
float roll
```
The roll component, basically rotation around the axis.
```c#
float yaw
```
The yaw component, typically left/right.
## Properties

```c#
static Angles Random { get; } 
```
Returns the angles of a uniformly random rotation.
```c#
Vector3 Forward { get; set; } 
```
The forward direction vector for this angle.
```c#
Angles Normal { get; } 
```
Returns normalized version of this object, meaning the angle on each axis is normalized to range of (-180,180].
## Methods

```c#
static Vector3 AngleVector( Angles ang) 
```
Converts an angle to a forward vector.
```c#
static float ClampAngle( float v) 
```
Clamps the angle to range of [0, 360)
```c#
static Angles Lerp( Angles source, Angles target, float frac) 
```
Performs linear interpolation on the two given angle objects.
```c#
static float NormalizeAngle( float v) 
```
Normalizes the angle to range of (-180, 180]
```c#
static Angles Parse( string str) 
```
Given a string, try to convert this into an angles object. The format is "p,y,r".
```c#
static Angles Parse( string str, IFormatProvider provider) 
```
ImplementsIParsable`1.ParseGiven a string, try to convert this into an angles object. The format is "p,y,r".
```c#
static Angles Read( BinaryReader reader) 
```
Read an angles object from given binary reader.
```c#
static bool TryParse( string str, out Angles result) 
```
Given a string, try to convert this into an angles object. The format is "p,y,r".
```c#
static bool TryParse( string str, IFormatProvider provider, out Angles result) 
```
ImplementsIParsable`1.TryParseGiven a string, try to convert this into an angles object. The format is "p,y,r".
```c#
Vector3 AsVector3( ) 
```
Return as a Vector3, where x = pitch etc
```c#
Angles Clamped( ) 
```
Returns clamped version of this object, meaning the angle on each axis is transformed to range of [0,360).
```c#
bool IsNearlyZero( double tolerance = 5E-324) 
```
Returns true if this angles object's components are all nearly zero with given tolerance.
```c#
Angles LerpTo( Angles target, float frac) 
```
Performs linear interpolation on the two given angle objects.
```c#
Rotation ToRotation( ) 
```
Converts these Euler angles to a rotation. The angles will be normalized.
```c#
Angles WithPitch( float pitch) 
```
Returns this angles object with given pitch component.
```c#
Angles WithRoll( float roll) 
```
Returns this angles object with given roll component.
```c#
Angles WithYaw( float yaw) 
```
Returns this angles object with given yaw component.
```c#
void Write( BinaryWriter writer) 
```
Write this angles object to a System.IO.BinaryWriter.
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( Angles o) 
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
Angles +( Angles c1, Angles c2) 
```
No Summary
```c#
Angles +( Angles c1, Vector3 c2) 
```
No Summary
```c#
Angles /( Angles c1, float c2) 
```
No Summary
```c#
bool ==( Angles left, Angles right) 
```
No Summary
```c#
bool !=( Angles left, Angles right) 
```
No Summary
```c#
Angles *( Angles c1, float c2) 
```
No Summary
```c#
Angles -( Angles c1, Angles c2) 
```
No Summary
## Referencing Members

```c#
static Angles = Input.AnalogLook { get; set; } 
```
```c#
Angles = Rotation.Angles( ) 
```
```c#
static Angles = SandboxSystemExtensions.Angles( Random ) 
```
```c#
Angles = AsAccessor.Angles { get; set; } 
```
```c#
Angles = SceneCamera.Angles { get; set; } 
```
```c#
Angles = SceneObject.Angles { get; set; } 
```
```c#
Angles = SkyboxAccessor.Angles { get; set; } 
```
```c#
abstract Angles = EntityObject.Angles { get; set; } 
```
```c#
Angles = MapNode.Angles { get; set; } 
```
```c#
Angles = ModelBoxAOProxy.Angles { get; set; } 
```
```c#
Angles = ModelEyeOcclusion.Angles { get; set; } 
```
```c#
virtual Angles = Entity.AngularVelocity { get; set; } 
```
```c#
Angles = VrHand.AngularVelocity { get; } 
```
```c#
Angles = Vector3.EulerAngles { get; set; } 
```
```c#
Angles = PushVolumeEntity.ForceDirection { get; set; } 
```
```c#
static Rotation = Rotation.From( Angles ) 
```
```c#
Angles = RenderAttributes.GetAngles( in string, in Angles ) 
```
```c#
Angles = ButtonEntity.MoveDir { get; set; } 
```
```c#
Angles = DoorEntity.MoveDir { get; set; } 
```
```c#
Angles = PathPlatformEntity.MoveDir { get; set; } 
```
```c#
Angles = PlatformEntity.MoveDir { get; set; } 
```
```c#
Angles = Player.OriginalViewAngles { get; } 
```
```c#
static Angles = SandboxSystemExtensions.ReadAngles( BinaryReader ) 
```
```c#
bool = GizmoControls.Rotate( string, Angles, out Angles ) 
```
```c#
void Particles.SetOrientation( int, Angles ) 
```
```c#
Angles = AnglesProperty.Value { get; set; } 
```
```c#
static Angles = Vector3.VectorAngle( Vector3 ) 
```
```c#
Angles = Player.ViewAngles { get; set; } 
```
```c#
static void SandboxSystemExtensions.Write( BinaryWriter, Angles ) 
```
