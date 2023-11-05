# Vector4

## ```c#
Implements IEquatable<Vector4>, IParsable<Vector4>
```

## Summary

A 4-dimensional vector/point.
## Constructors

```c#
Vector4( float x, float y, float z, float w) 
```
Initializes a vector4 with given components.
```c#
Vector4( in Vector3 v, float w = 0) 
```
Initializes a 4D vector from given #D vector and the given W component.
```c#
Vector4( float all) 
```
Initializes the 4D vector with all components set to given value.
## Fields

```c#
static readonly Vector4 One
```
A 4D vector with all components set to 1.
```c#
static readonly Vector4 Zero
```
A 4D vector with all components set to 0.
## Properties

```c#
bool IsNearZeroLength { get; } 
```
Whether length of this vector is nearly zero.
```c#
float Length { get; } 
```
The length of this vector object
```c#
float LengthSquared { get; } 
```
The squared length of this vector object
```c#
float w { get; set; } 
```
The W component of this Vector.
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
static Vector4 Lerp( Vector4 a, Vector4 b, float frac, bool clamp = true) 
```
Performs linear interpolation between 2 given vectors.
```c#
static Vector4 Parse( string str) 
```
Given a string, try to convert this into a vector4. The format is "x,y,z,w".
```c#
static Vector4 Parse( string str, IFormatProvider provider) 
```
ImplementsIParsable`1.ParseGiven a string, try to convert this into a vector4. The format is "x,y,z,w".
```c#
static bool TryParse( string str, out Vector4 result) 
```
Given a string, try to convert this into a vector4. The format is "x,y,z,w".
```c#
static bool TryParse( string str, IFormatProvider provider, out Vector4 result) 
```
ImplementsIParsable`1.TryParseGiven a string, try to convert this into a vector4. The format is "x,y,z,w".
```c#
Vector4 LerpTo( Vector4 target, float frac, bool clamp = true) 
```
Performs linear interpolation between this and given vectors.
```c#
override bool Equals( Vector4 other) 
```
OverridesValueType.Equals
```c#
override string ToString( ) 
```
OverridesValueType.ToStringFormats the Vector into a string "x,y,z,w"
## Operators

```c#
Vector4 +( in Vector4 c1, in Vector4 c2) 
```
No Summary
```c#
Vector4 /( in Vector4 c1, float f) 
```
No Summary
```c#
Vector4 *( in Vector4 c1, float f) 
```
No Summary
```c#
Vector4 *( in Vector4 c1, in Vector4 c2) 
```
No Summary
```c#
Vector4 *( float f, in Vector4 c1) 
```
No Summary
```c#
Vector4 -( in Vector4 c1, in Vector4 c2) 
```
No Summary
```c#
Vector4 -( in Vector4 value) 
```
No Summary
```c#
implicit Vector4 =( Vector4 value) 
```
No Summary
```c#
implicit Vector4 =( Vector4 value) 
```
No Summary
```c#
implicit Vector4 =( in Color value) 
```
No Summary
## Referencing Members

```c#
Vector4 = VertexDetail.Color { get; set; } 
```
```c#
Vector4 = ShatterGlass.FaceAxisU { get; set; } 
```
```c#
Vector4 = VoxelSurface.FaceAxisU { get; set; } 
```
```c#
Vector4 = ShatterGlass.FaceAxisV { get; set; } 
```
```c#
Vector4 = VoxelSurface.FaceAxisV { get; set; } 
```
```c#
static Vector4 = SandboxSystemExtensions.Gaussian4D( Random, Vector4?, Vector4? ) 
```
```c#
static Vector4 = SandboxSystemExtensions.Gaussian4D( Random, Vector4?, Vector4? ) 
```
```c#
Vector4 = RenderAttributes.GetVector4( in string, in Vector4 ) 
```
```c#
static Color = Color.op_Implicit( Vector4 ) 
```
```c#
static Vector4 = Vector2.op_Implicit( Vector2 ) 
```
```c#
static Vector3 = Vector3.op_Implicit( Vector4 ) 
```
```c#
Vector4 = VertexDetail.Paint0 { get; set; } 
```
```c#
Vector4 = VertexDetail.Paint1 { get; set; } 
```
```c#
bool = Material.Set( string, Vector4 ) 
```
```c#
Vector4 = Vertex.Tangent
```
```c#
Vector4 = Vertex.TexCoord0
```
```c#
Vector4 = Vertex.TexCoord1
```
```c#
Vector4 = Rect.ToVector4( ) 
```
```c#
Vertex.Vertex( Vector3, Vector4, Color32 ) 
```
```c#
Vertex.Vertex( Vector3, Vector3, Vector3, Vector4 ) 
```
