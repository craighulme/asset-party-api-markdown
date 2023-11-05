# PanelTransform

## ```c#
Derives from ValueType
```

## Summary

Returns true if this is empty.
## Fields

```c#
ImmutableList<Entry> List
```
No Summary
## Properties

```c#
int Entries { get; } 
```
No Summary
## Methods

```c#
bool AddMatrix3D( Matrix matrix) 
```
No Summary
```c#
bool AddPerspective( Length d) 
```
No Summary
```c#
bool AddRotation( float x, float y, float z) 
```
No Summary
```c#
bool AddRotation( Vector3 angles) 
```
No Summary
```c#
bool AddScale( float scale) 
```
No Summary
```c#
bool AddScale( Vector3 scale) 
```
No Summary
```c#
bool AddSkew( float x, float y, float z) 
```
No Summary
```c#
bool AddTranslate( Length? lengthX, Length? lengthY, Length? lengthZ = null) 
```
No Summary
```c#
bool AddTranslateX( Length? length) 
```
No Summary
```c#
bool AddTranslateY( Length? length) 
```
No Summary
```c#
bool AddTranslateZ( Length? length) 
```
No Summary
```c#
Matrix BuildTransform( float width, float height, Vector2 perspectiveOrigin) 
```
No Summary
```c#
bool IsEmpty( ) 
```
Returns true if this is empty.
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override int GetHashCode( ) 
```
OverridesValueType.GetHashCode
## Operators

```c#
bool ==( PanelTransform a, PanelTransform b) 
```
No Summary
```c#
bool !=( PanelTransform a, PanelTransform b) 
```
No Summary
## Nested Types

## Referencing Members

```c#
protected void BaseStyles.Lerp( string, ref PanelTransform?, PanelTransform?, PanelTransform?, PanelTransform?, float ) 
```
```c#
PanelTransform? = BaseStyles.Transform { get; set; } 
```
