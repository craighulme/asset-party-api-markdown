# RenderTarget

## 
```c#
Implements IDisposable
```

## Summary

Essentially wraps a couple of textures that we're going to render to. The color texture and the depth texture.
## Constructors

```c#
RenderTarget( ) 
```
No Summary
## Properties

```c#
Texture ColorTarget { get; } 
```
The target colour texture
```c#
Texture DepthTarget { get; } 
```
The target depth texture
```c#
int Height { get; } 
```
Height of the render target
```c#
int Width { get; } 
```
Width of the render target
## Methods

```c#
static RenderTarget From( Texture color, Texture depth = null) 
```
Create a render target from these textures
```c#
static RenderTarget GetTemporary( int width, int height, ImageFormat colorFormat, ImageFormat depthFormat, MultisampleAmount msaa, int numMips) 
```
Get a temporary render target. You should dispose the returned handle when you're done to return the textures to the pool.
```c#
static RenderTarget GetTemporary( int sizeFactor, ImageFormat colorFormat, ImageFormat depthFormat, MultisampleAmount msaa, int numMips) 
```
Get a temporary render target. You should dispose the returned handle when you're done to return the textures to the pool.
```c#
static RenderTarget GetTemporary( int width, int height, ImageFormat colorFormat = -2, ImageFormat depthFormat = -2, int msaa = 0) 
```
No Summary
```c#
static RenderTarget GetTemporary( int sizeFactor = 1, ImageFormat colorFormat = -2, ImageFormat depthFormat = -2, int msaa = 0) 
```
No Summary
```c#
virtual void Dispose( ) 
```
ImplementsIDisposable.DisposeStop using this texture, return it to the pool
```c#
override string ToString( ) 
```
OverridesObject.ToString
