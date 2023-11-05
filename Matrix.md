# Matrix

## 
```c#
Implements IEquatable<Matrix>
```

## Summary

Represents a 4x4 matrix.
## Fields

```c#
Matrix4x4 Numerics
```
No Summary
## Properties

```c#
static Matrix Identity { get; } 
```
Returns the multiplicative identity matrix.
```c#
Matrix Inverted { get; } 
```
Returns inverse of this matrix.
## Methods

```c#
static Matrix CreateMatrix3D( float[] matrix) 
```
No Summary
```c#
static Matrix CreateRotation( Rotation rot) 
```
No Summary
```c#
static Matrix CreateRotation( Vector3 angles) 
```
No Summary
```c#
static Matrix CreateRotationX( float degrees) 
```
No Summary
```c#
static Matrix CreateRotationX( float degrees, Vector3 center) 
```
No Summary
```c#
static Matrix CreateRotationY( float degrees) 
```
No Summary
```c#
static Matrix CreateRotationY( float degrees, Vector3 center) 
```
No Summary
```c#
static Matrix CreateRotationZ( float degrees) 
```
No Summary
```c#
static Matrix CreateRotationZ( float degrees, Vector3 center) 
```
No Summary
```c#
static Matrix CreateScale( Vector3 scales) 
```
No Summary
```c#
static Matrix CreateScale( Vector3 scales, Vector3 centerPoint) 
```
No Summary
```c#
static Matrix CreateSkew( Vector2 skew) 
```
No Summary
```c#
static Matrix CreateSkewX( float degrees) 
```
No Summary
```c#
static Matrix CreateSkewY( float degrees) 
```
No Summary
```c#
static Matrix CreateTranslation( Vector3 vec) 
```
No Summary
```c#
static Matrix CreateWorld( Vector3 position, Vector3 forward, Vector3 up) 
```
No Summary
```c#
static Matrix Lerp( Matrix ma, Matrix mb, float frac) 
```
Performs linear interpolation from one matrix to another.
```c#
static Matrix Slerp( Matrix ma, Matrix mb, float frac) 
```
Performs spherical interpolation from one matrix to another.
```c#
Vector3 Transform( Vector3 v) 
```
Transforms a vector by a 4x4 matrix
```c#
Vector3 TransformNormal( Vector3 v) 
```
Transforms a normal vector by a specified 4x4 matrix
```c#
Matrix Transpose( ) 
```
Returns transposed version of this matrix, meaning columns in this matrix become rows in the returned matrix and rows in this matrix become columns in the returned one.
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( Matrix o) 
```
OverridesValueType.Equals
```c#
override int GetHashCode( ) 
```
OverridesValueType.GetHashCode
```c#
override string ToString( ) 
```
OverridesValueType.ToStringFormats the matrix and returns it as a string.
## Operators

```c#
bool ==( Matrix left, Matrix right) 
```
No Summary
```c#
bool !=( Matrix left, Matrix right) 
```
No Summary
```c#
Matrix *( Matrix value1, Matrix value2) 
```
No Summary
```c#
implicit Matrix =( Matrix4x4 value) 
```
No Summary
```c#
implicit Matrix4x4 =( Matrix value) 
```
No Summary
## Referencing Members

```c#
bool = PanelTransform.AddMatrix3D( Matrix ) 
```
```c#
Matrix = PanelTransform.BuildTransform( float, float, Vector2 ) 
```
```c#
Matrix = Styles.BuildTransformMatrix( Vector2 ) 
```
```c#
abstract Matrix? = IPanel.GlobalMatrix { get; } 
```
```c#
Matrix? = Panel.GlobalMatrix { get; } 
```
```c#
Matrix? = Panel.LocalMatrix { get; } 
```
```c#
Matrix = Entry.Matrix
```
```c#
Matrix = PlanarReflection.ReflectMatrix( Matrix, Plane ) 
```
```c#
Matrix = PlanarReflection.ReflectMatrix( Matrix, Plane ) 
```
```c#
Matrix = Entry.ToMatrix( float, float ) 
```
