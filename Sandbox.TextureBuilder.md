# TextureBuilder

## ```c#
Derives from ValueType
```

## Summary

Finish creating the texture.
## Methods

```c#
Texture Create( string name = null, bool anonymous = true, ReadOnlySpan<byte> data = null, int dataLength = 0) 
```
Finish creating the texture.
```c#
TextureBuilder WithDepth( int depth) 
```
No Summary
```c#
TextureBuilder WithDepthFormat( ) 
```
Uses the same depth format as what the screen/framebuffer uses.
```c#
TextureBuilder WithDynamicUsage( ) 
```
Provides a hint to the GPU that this texture will be updated regularly. (almost every frame)
```c#
TextureBuilder WithFormat( ImageFormat format) 
```
The internal texture format to use.
```c#
TextureBuilder WithGPUOnlyUsage( ) 
```
Specify the texture to ONLY be used on the GPU on not allow CPU access.
```c#
TextureBuilder WithHeight( int height) 
```
No Summary
```c#
TextureBuilder WithMips( int mips) 
```
Generate amount of mip levels.
```c#
TextureBuilder WithMSAA( MultisampleAmount amount) 
```
No Summary
```c#
TextureBuilder WithMSAA( int amount) 
```
No Summary
```c#
TextureBuilder WithMultiSample16X( ) 
```
Sets the texture to use 16x multisampling.
```c#
TextureBuilder WithMultiSample2X( ) 
```
Sets the texture to use 2x multisampling.
```c#
TextureBuilder WithMultiSample4X( ) 
```
Sets the texture to use 4x multisampling.
```c#
TextureBuilder WithMultiSample6X( ) 
```
Sets the texture to use 6x multisampling.
```c#
TextureBuilder WithMultiSample8X( ) 
```
Sets the texture to use 8x multisampling.
```c#
TextureBuilder WithScreenFormat( ) 
```
Sets the internal texture format to use the same format as the screen/frame buffer.
```c#
TextureBuilder WithScreenMultiSample( ) 
```
Sets the texture to use the same multisampling as whatever the screen/framebuffer uses
```c#
TextureBuilder WithSemiStaticUsage( ) 
```
Provides a hint to the GPU that this texture will only be updated sometimes.
```c#
TextureBuilder WithSize( int width, int height) 
```
No Summary
```c#
TextureBuilder WithSize( Vector2 size) 
```
No Summary
```c#
TextureBuilder WithStaticUsage( ) 
```
Provides a hint to the GPU that this texture will not be modified.
```c#
TextureBuilder WithUAVBinding( bool uav) 
```
Support binding the texture as a Unordered Access View in a compute or pixel shader.
This is required for binding a texture within a compute shader
```c#
TextureBuilder WithUAVBinding( ) 
```
No Summary
```c#
TextureBuilder WithWidth( int width) 
```
No Summary
## Referencing Members

```c#
static TextureBuilder = Texture.CreateCustom( ) 
```
```c#
static TextureBuilder = Texture.CreateRenderTarget( ) 
```
