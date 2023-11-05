# Texture2DBuilder

## Derives from ValueType

## Summary

Build and create the actual texture
## Constructors

```c#
Texture2DBuilder( ) 
```
No Summary
## Methods

```c#
Texture Finish( ) 
```
Build and create the actual texture
```c#
Texture2DBuilder WithAnonymous( bool isAnonymous) 
```
Set whether the texture is an anonymous texture or not
```c#
Texture2DBuilder WithData( byte[] data) 
```
Initialize texture with pre-existing texture data.
```c#
Texture2DBuilder WithData( byte[] data, int dataLength) 
```
Initialize texture with pre-existing texture data.
```c#
Texture2DBuilder WithDepthFormat( ) 
```
Uses the same depth format as what the screen/framebuffer uses.
```c#
Texture2DBuilder WithDynamicUsage( ) 
```
Provides a hint to the GPU that this texture will be updated regularly. (almost every frame)
```c#
Texture2DBuilder WithFormat( ImageFormat format) 
```
The internal texture format to use.
```c#
Texture2DBuilder WithGPUOnlyUsage( ) 
```
Specify the texture to ONLY be used on the GPU on not allow CPU access.
```c#
Texture2DBuilder WithMips( int mips) 
```
Generate amount of mip levels.
```c#
Texture2DBuilder WithMultisample( MultisampleAmount amount) 
```
Use Multi-Sample Anti Aliasing (MSAA) of given sample count.
```c#
Texture2DBuilder WithMultiSample16X( ) 
```
Sets the texture to use 16x multisampling.
```c#
Texture2DBuilder WithMultiSample2X( ) 
```
Sets the texture to use 2x multisampling.
```c#
Texture2DBuilder WithMultiSample4X( ) 
```
Sets the texture to use 4x multisampling.
```c#
Texture2DBuilder WithMultiSample6X( ) 
```
Sets the texture to use 6x multisampling.
```c#
Texture2DBuilder WithMultiSample8X( ) 
```
Sets the texture to use 8x multisampling.
```c#
Texture2DBuilder WithName( string name) 
```
Provide a name to identify the texture by
```c#
Texture2DBuilder WithScreenFormat( ) 
```
Sets the internal texture format to use the same format as the screen/frame buffer.
```c#
Texture2DBuilder WithScreenMultiSample( ) 
```
Sets the texture to use the same multisampling as whatever the screen/framebuffer uses
```c#
Texture2DBuilder WithSemiStaticUsage( ) 
```
Provides a hint to the GPU that this texture will only be updated sometimes.
```c#
Texture2DBuilder WithSize( int width, int height) 
```
Create texture with a predefined size.
```c#
Texture2DBuilder WithSize( Vector2 size) 
```
Create texture with a predefined size
```c#
Texture2DBuilder WithStaticUsage( ) 
```
Provides a hint to the GPU that this texture will not be modified.
```c#
Texture2DBuilder WithUAVBinding( ) 
```
Support binding the texture as a Unordered Access View in a compute or pixel shader.
This is required for binding a texture within a compute shader
## Referencing Members

```c#
static Texture2DBuilder = Texture.Create( int, int, ImageFormat ) 
```
