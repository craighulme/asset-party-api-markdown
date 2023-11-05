# Color32

## ```c#
Implements IEquatable<Color32>
```

## Summary

A 32bit color, commonly used by things like vertex buffers.The functionality on this is purposely left minimal so we're encouraged to use the regularColorstruct.
## Constructors

```c#
Color32( byte r, byte g, byte b, byte a = 255) 
```
Initialize a color with each component set to given values, in range [0,255]
```c#
Color32( byte all) 
```
Initialize a color with each component set to given value, even alpha.
```c#
Color32( uint raw) 
```
Initialize from an integer of the form 0xAABBGGRR.
```c#
Color32( int raw) 
```
Initialize from an integer of the form 0xAABBGGRR.
## Fields

```c#
byte a
```
The alpha/transparency color component, in range of 0 (fully transparent) to 255 (fully opaque).
```c#
byte b
```
The blue color component, in range of 0-255.
```c#
byte g
```
The green color component, in range of 0-255.
```c#
byte r
```
The red color component, in range of 0-255.
## Properties

```c#
static Color32 Black { get; } 
```
A constant representing a fully opaque color black.
```c#
static Color32 Transparent { get; } 
```
A constant representing a fully transparent color.
```c#
static Color32 White { get; } 
```
A constant representing a fully opaque color white.
```c#
string Hex { get; } 
```
String representation of the form "#RRGGBB[AA]".
```c#
uint RawInt { get; } 
```
Integer representation of the form 0xAABBGGRR as used by native code.
```c#
string Rgb { get; } 
```
String representation in the form ofrgb( r, g, b )
css function notation.
```c#
string Rgba { get; } 
```
String representation in the form ofrgba( r, g, b, a )
css function notation.
```c#
uint RgbaInt { get; } 
```
Integer representation of the form 0xRRGGBBAA.
```c#
uint RgbInt { get; } 
```
Integer representation of the form 0xRRGGBB.
## Methods

```c#
static Color32 FromRgb( uint rgb) 
```
Converts an integer of the form 0xRRGGBB into the color #RRGGBB with 100% alpha.
```c#
static Color32 FromRgba( uint rgba) 
```
Converts an integer of the form 0xRRGGBBAA into the color #RRGGBBAA.
```c#
static Color32 Max( Color32 a, Color32 b) 
```
Returns a new color with each component being the maximum of the 2 given colors.
```c#
static Color32 Min( Color32 a, Color32 b) 
```
Returns a new color with each component being the minimum of the 2 given colors.
```c#
static Color32? Parse( string value) 
```
Parse a string to a color, in format "255 255 255 255" or "255,255,255". Alpha is optional.
```c#
static Color32 Read( BinaryReader reader) 
```
Read a color from binary reader.
```c#
Color ToColor( ) 
```
Convert this object toColor.
```c#
Color ToColor( bool srgb) 
```
Convert this object toColor.
```c#
void Write( BinaryWriter writer) 
```
Write this color to a binary writer.
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( Color32 o) 
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
bool ==( Color32 left, Color32 right) 
```
No Summary
```c#
bool !=( Color32 left, Color32 right) 
```
No Summary
```c#
implicit Color32 =( Color value) 
```
No Summary
## Referencing Members

```c#
static void SandboxBaseExtensions.AddCube( VertexBuffer, Vector3, Vector3, Rotation, Color32 ) 
```
```c#
Color32 = SphereAttribute.Color { get; set; } 
```
```c#
Color32 = Vertex.Color
```
```c#
Color32 = Texture.GetPixel( float, float, int ) 
```
```c#
Color32 = Texture.GetPixel3D( float, float, float, int ) 
```
```c#
static Color = Color.op_Implicit( Color32 ) 
```
```c#
Color32 = Color.ToColor32( bool ) 
```
```c#
void Texture.Update( ReadOnlySpan<Color32>, int, int, int, int ) 
```
```c#
void Texture.Update( Color32, Rect ) 
```
```c#
void Texture.Update( Color32, float, float ) 
```
```c#
Vertex.Vertex( Vector3, Color32 ) 
```
```c#
Vertex.Vertex( Vector3, Vector4, Color32 ) 
```
