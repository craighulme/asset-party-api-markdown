# Material

## ```c#
Derives from Resource
```

## Summary

A material. Uses severalSandbox.Textures and aSandbox.Shaderwith specific settings for more interesting visual effects.
## Properties

```c#
RenderAttributes Attributes { get; } 
```
Access to all of the attributes of this material.
```c#
Texture FirstTexture { get; } 
```
No Summary
```c#
string Name { get; } 
```
Name (or path) of the material.
## Methods

```c#
static Material Create( string materialName, string shader) 
```
Create a new empty material at runtime.
```c#
static Material FromShader( Shader shader) 
```
Get an empty material based on the specified shader. This will cache the material so that subsequent calls
will return the same material.
```c#
static Material FromShader( string path) 
```
Get an empty material based on the specified shader. This will cache the material so that subsequent calls
will return the same material.
```c#
static Material Load( string filename) 
```
Load a material from disk. Has internal cache.
```c#
Material CreateCopy( ) 
```
Create a copy of this material
```c#
Texture GetTexture( string name) 
```
No Summary
```c#
bool Set( string param, Vector4 value) 
```
Overrides/Sets an Vector4 within the material
```c#
bool Set( string param, Texture texture) 
```
Override/Sets texture parameter (Color, Normal, etc)
```c#
bool Set( string param, Color value) 
```
Overrides/Sets an color within the material as a color value within the material
```c#
bool Set( string param, Vector3 value) 
```
Overrides/Sets an Vector3 within the material
```c#
bool Set( string param, Vector2 value) 
```
Overrides/Sets an Vector2 within the material
```c#
bool Set( string param, float value) 
```
Overrides/Sets an float within the material
```c#
bool Set( string param, int value) 
```
Overrides/Sets an int within the material
```c#
bool Set( string param, bool value) 
```
Overrides/Sets an bool within the material
## Nested Types

