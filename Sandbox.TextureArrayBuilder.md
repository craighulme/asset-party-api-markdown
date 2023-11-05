# TextureArrayBuilder

## Derives from ValueType

## Summary

Build and create the actual texture
## Constructors

```c#
TextureArrayBuilder( ) 
```
No Summary
## Methods

```c#
Texture Finish( ) 
```
Build and create the actual texture
```c#
TextureArrayBuilder WithAnonymous( bool isAnonymous) 
```
Set whether the texture is an anonymous texture or not
```c#
TextureArrayBuilder WithCount( int count = 1) 
```
Create texture array with this many textures
```c#
TextureArrayBuilder WithData( byte[] data) 
```
Initialize texture with pre-existing texture data
```c#
TextureArrayBuilder WithData( byte[] data, int dataLength) 
```
Initialize texture with pre-existing texture data
```c#
TextureArrayBuilder WithDepthFormat( ) 
```
Uses the same depth format as what the screen/framebuffer uses.
```c#
TextureArrayBuilder WithDynamicUsage( ) 
```
Provides a hint to the GPU that this texture will be updated regularly. (almost every frame)
```c#
TextureArrayBuilder WithFormat( ImageFormat format) 
```
The internal texture format to use.
```c#
TextureArrayBuilder WithGPUOnlyUsage( ) 
```
Specify the texture to ONLY be used on the GPU on not allow CPU access.
```c#
TextureArrayBuilder WithMips( int mips) 
```
Generate amount of mip levels.
```c#
TextureArrayBuilder WithMultisample( MultisampleAmount amount) 
```
Define which how much multisampling the current texture should use
```c#
TextureArrayBuilder WithMultiSample16X( ) 
```
Sets the texture to use 16x multisampling.
```c#
TextureArrayBuilder WithMultiSample2X( ) 
```
Sets the texture to use 2x multisampling.
```c#
TextureArrayBuilder WithMultiSample4X( ) 
```
Sets the texture to use 4x multisampling.
```c#
TextureArrayBuilder WithMultiSample6X( ) 
```
Sets the texture to use 6x multisampling.
```c#
TextureArrayBuilder WithMultiSample8X( ) 
```
Sets the texture to use 8x multisampling.
```c#
TextureArrayBuilder WithName( string name) 
```
Provide a name to identify the texture by
```c#
TextureArrayBuilder WithScreenFormat( ) 
```
Sets the internal texture format to use the same format as the screen/frame buffer.
```c#
TextureArrayBuilder WithScreenMultiSample( ) 
```
Sets the texture to use the same multisampling as whatever the screen/framebuffer uses
```c#
TextureArrayBuilder WithSemiStaticUsage( ) 
```
Provides a hint to the GPU that this texture will only be updated sometimes.
```c#
TextureArrayBuilder WithSize( int width = 1, int height = 1) 
```
Create texture with a predefined size
```c#
TextureArrayBuilder WithStaticUsage( ) 
```
Provides a hint to the GPU that this texture will not be modified.
```c#
TextureArrayBuilder WithUAVBinding( ) 
```
Support binding the texture as a Unordered Access View in a compute or pixel shader.
This is required for binding a texture within a compute shader
## Referencing Members

```c#
static TextureArrayBuilder = Texture.CreateArray( int, int, int, ImageFormat ) 
```
