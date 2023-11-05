# Texture3DBuilder

## Derives from ValueType

## Summary

Build and create the actual texture
## Constructors

```c#
Texture3DBuilder( ) 
```
No Summary
## Methods

```c#
Texture Finish( ) 
```
Build and create the actual texture
```c#
Texture3DBuilder WithAnonymous( bool isAnonymous) 
```
Set whether the texture is an anonymous texture or not
```c#
Texture3DBuilder WithData( byte[] data) 
```
Initialize texture with pre-existing texture data
```c#
Texture3DBuilder WithData( byte[] data, int dataLength) 
```
Initialize texture with pre-existing texture data
```c#
Texture3DBuilder WithDepthFormat( ) 
```
Uses the same depth format as what the screen/framebuffer uses.
```c#
Texture3DBuilder WithDynamicUsage( ) 
```
Provides a hint to the GPU that this texture will be updated regularly. (almost every frame)
```c#
Texture3DBuilder WithFormat( ImageFormat format) 
```
The internal texture format to use.
```c#
Texture3DBuilder WithGPUOnlyUsage( ) 
```
Specify the texture to ONLY be used on the GPU on not allow CPU access.
```c#
Texture3DBuilder WithMips( int mips) 
```
Generate amount of mip levels.
```c#
Texture3DBuilder WithMultisample( MultisampleAmount amount) 
```
Define which how much multisampling the current texture should use
```c#
Texture3DBuilder WithMultiSample16X( ) 
```
Sets the texture to use 16x multisampling.
```c#
Texture3DBuilder WithMultiSample2X( ) 
```
Sets the texture to use 2x multisampling.
```c#
Texture3DBuilder WithMultiSample4X( ) 
```
Sets the texture to use 4x multisampling.
```c#
Texture3DBuilder WithMultiSample6X( ) 
```
Sets the texture to use 6x multisampling.
```c#
Texture3DBuilder WithMultiSample8X( ) 
```
Sets the texture to use 8x multisampling.
```c#
Texture3DBuilder WithName( string name) 
```
Provide a name to identify the texture by
```c#
Texture3DBuilder WithScreenFormat( ) 
```
Sets the internal texture format to use the same format as the screen/frame buffer.
```c#
Texture3DBuilder WithScreenMultiSample( ) 
```
Sets the texture to use the same multisampling as whatever the screen/framebuffer uses
```c#
Texture3DBuilder WithSemiStaticUsage( ) 
```
Provides a hint to the GPU that this texture will only be updated sometimes.
```c#
Texture3DBuilder WithSize( int width = 1, int height = 1, int depth = 1) 
```
Create texture with a predefined size
```c#
Texture3DBuilder WithSize( Vector3 size) 
```
Create texture with a predefined size
```c#
Texture3DBuilder WithStaticUsage( ) 
```
Provides a hint to the GPU that this texture will not be modified.
```c#
Texture3DBuilder WithUAVBinding( ) 
```
Support binding the texture as a Unordered Access View in a compute or pixel shader.
This is required for binding a texture within a compute shader
## Referencing Members

```c#
static Texture3DBuilder = Texture.CreateVolume( int, int, int, ImageFormat ) 
```
