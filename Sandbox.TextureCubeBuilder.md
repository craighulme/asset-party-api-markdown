# TextureCubeBuilder

## Derives from ValueType

## Summary

Build and create the actual texture
## Constructors

```c#
TextureCubeBuilder( ) 
```
No Summary
## Methods

```c#
Texture Finish( ) 
```
Build and create the actual texture
```c#
TextureCubeBuilder WithAnonymous( bool isAnonymous) 
```
Set whether the texture is an anonymous texture or not
```c#
TextureCubeBuilder WithData( byte[] data) 
```
Initialize texture with pre-existing texture data
```c#
TextureCubeBuilder WithData( byte[] data, int dataLength) 
```
Initialize texture with pre-existing texture data
```c#
TextureCubeBuilder WithDepthFormat( ) 
```
Uses the same depth format as what the screen/framebuffer uses.
```c#
TextureCubeBuilder WithDynamicUsage( ) 
```
Provides a hint to the GPU that this texture will be updated regularly. (almost every frame)
```c#
TextureCubeBuilder WithFormat( ImageFormat format) 
```
The internal texture format to use.
```c#
TextureCubeBuilder WithGPUOnlyUsage( ) 
```
Specify the texture to ONLY be used on the GPU on not allow CPU access.
```c#
TextureCubeBuilder WithMultisample( MultisampleAmount amount) 
```
Define which how much multisampling the current texture should use
```c#
TextureCubeBuilder WithMultiSample16X( ) 
```
Sets the texture to use 16x multisampling.
```c#
TextureCubeBuilder WithMultiSample2X( ) 
```
Sets the texture to use 2x multisampling.
```c#
TextureCubeBuilder WithMultiSample4X( ) 
```
Sets the texture to use 4x multisampling.
```c#
TextureCubeBuilder WithMultiSample6X( ) 
```
Sets the texture to use 6x multisampling.
```c#
TextureCubeBuilder WithMultiSample8X( ) 
```
Sets the texture to use 8x multisampling.
```c#
TextureCubeBuilder WithName( string name) 
```
Provide a name to identify the texture by
```c#
TextureCubeBuilder WithScreenFormat( ) 
```
Sets the internal texture format to use the same format as the screen/frame buffer.
```c#
TextureCubeBuilder WithScreenMultiSample( ) 
```
Sets the texture to use the same multisampling as whatever the screen/framebuffer uses
```c#
TextureCubeBuilder WithSemiStaticUsage( ) 
```
Provides a hint to the GPU that this texture will only be updated sometimes.
```c#
TextureCubeBuilder WithSize( int width, int height) 
```
Create texture with a predefined size
```c#
TextureCubeBuilder WithSize( Vector2 size) 
```
Create texture with a predefined size
```c#
TextureCubeBuilder WithStaticUsage( ) 
```
Provides a hint to the GPU that this texture will not be modified.
```c#
TextureCubeBuilder WithUAVBinding( ) 
```
Support binding the texture as a Unordered Access View in a compute or pixel shader.
This is required for binding a texture within a compute shader
## Referencing Members

```c#
static TextureCubeBuilder = Texture.CreateCube( int, int, ImageFormat ) 
```
