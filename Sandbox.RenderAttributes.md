# RenderAttributes

## 
```c#
Derives from object
```

## Summary

Get a vector4 value - else defaultValue if missing
## Constructors

```c#
RenderAttributes( ) 
```
No Summary
## Methods

```c#
void Clear( ) 
```
No Summary
```c#
Angles GetAngles( in string name, in Angles defaultValue = null) 
```
Get a vector4 value - else defaultValue if missing
```c#
bool GetBool( in string name, in bool defaultValue = false) 
```
Get a bool value - else defaultValue if missing
```c#
bool GetComboBool( in string k, in bool defaultValue = false) 
```
No Summary
```c#
T GetComboEnum<T,>( in string k, in T defaultValue) 
```
No Summary
```c#
int GetComboInt( in string k, in int defaultValue = 0) 
```
No Summary
```c#
float GetFloat( in string name, in float defaultValue = 0) 
```
Get a float value - else defaultValue if missing
```c#
int GetInt( in string name, in int defaultValue = 0) 
```
Get a int value - else defaultValue if missing
```c#
Texture GetTexture( in string name, in Texture defaultValue = null) 
```
Get a texture value - else defaultValue if missing
```c#
Vector3 GetVector( in string name, in Vector3 defaultValue = null) 
```
Get a vector3 value - else defaultValue if missing
```c#
Vector4 GetVector4( in string name, in Vector4 defaultValue = null) 
```
Get a vector4 value - else defaultValue if missing
```c#
void Set( in string k, in int value) 
```
No Summary
```c#
void Set( in string k, in Texture value, in int mip = -1) 
```
No Summary
```c#
void Set( in string k, in float value) 
```
No Summary
```c#
void Set( in string k, in string value) 
```
No Summary
```c#
void Set( in string k, in bool value) 
```
No Summary
```c#
void Set( in string k, in Vector4 value) 
```
No Summary
```c#
void Set( in string k, in Angles value) 
```
No Summary
```c#
void Set( in string k, in Vector3 value) 
```
No Summary
```c#
void Set( in string k, in Vector2 value) 
```
No Summary
```c#
void Set<T,>( in string k, in ComputeBuffer<T> value) 
```
No Summary
```c#
void Set( in string k, in Matrix value) 
```
No Summary
```c#
void SetCombo( in string k, in int value) 
```
No Summary
```c#
void SetCombo( in string k, in Enum value) 
```
No Summary
```c#
void SetCombo( in string k, in bool value) 
```
No Summary
```c#
void SetData<T,>( in string k, Span<T> value) 
```
Set a constant buffer to a specific value
```c#
void SetData<T,>( in string k, T value) 
```
Set a constant buffer to a specific value
```c#
void SetData<T,>( in string k, T[] value) 
```
Set a constant buffer to a specific value
```c#
void SetData<T,>( in string k, List<T> value) 
```
Set a constant buffer to a specific value
