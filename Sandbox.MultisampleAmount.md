# MultisampleAmount

## ```c#
Derives from Enum
```

## Summary

No Summary
## Fields

```c#
static MultisampleAmount Multisample16x = 4
```
No Summary
```c#
static MultisampleAmount Multisample2x = 0
```
No Summary
```c#
static MultisampleAmount Multisample4x = 1
```
No Summary
```c#
static MultisampleAmount Multisample6x = 2
```
No Summary
```c#
static MultisampleAmount Multisample8x = 3
```
No Summary
```c#
static MultisampleAmount MultisampleNone = 6
```
No Summary
```c#
static MultisampleAmount MultisampleScreen = 5
```
No Summary
## Referencing Members

```c#
static RenderTarget = RenderTarget.GetTemporary( int, int, ImageFormat, ImageFormat, MultisampleAmount, int ) 
```
```c#
static RenderTarget = RenderTarget.GetTemporary( int, ImageFormat, ImageFormat, MultisampleAmount, int ) 
```
```c#
TextureBuilder = TextureBuilder.WithMSAA( MultisampleAmount ) 
```
```c#
Texture2DBuilder = Texture2DBuilder.WithMultisample( MultisampleAmount ) 
```
```c#
Texture3DBuilder = Texture3DBuilder.WithMultisample( MultisampleAmount ) 
```
```c#
TextureArrayBuilder = TextureArrayBuilder.WithMultisample( MultisampleAmount ) 
```
```c#
TextureCubeBuilder = TextureCubeBuilder.WithMultisample( MultisampleAmount ) 
```
