# Texture

## 
```c#
Implements IDisposable
```

## Summary

A texture is an image used in rendering. Can be a static texture loaded from disk, or a dynamic texture rendered to by code.
Can also be 2D, 3D (multiple slices), or a cube texture (6 slices).
## Properties

```c#
static Texture Invalid { get; } 
```
1x1 solid magenta colored texture.
```c#
static Texture Transparent { get; } 
```
1x1 fully transparent texture.
```c#
static Texture White { get; } 
```
1x1 solid white opaque texture.
```c#
int Depth { get; } 
```
Depth of a 3D texture in pixels, or slice count for 2D texture arrays.
```c#
int Height { get; } 
```
Height of the texture in pixels.
```c#
ImageFormat ImageFormat { get; } 
```
Image format of this texture.
```c#
bool IsLoaded { get; } 
```
Whether this texture has finished loading or not.
```c#
int LastUsed { get; } 
```
Returns how many frames ago this texture was last used by the renderer
```c#
int Mips { get; } 
```
Number ofmip mapsthis texture has.
```c#
Vector2 Size { get; } 
```
Returns a Vector2 representing the size of the texture (width, height)
```c#
int Width { get; } 
```
Width of the texture in pixels.
## Methods

```c#
static Texture2DBuilder Create( int width, int height, ImageFormat format = 0) 
```
Begins creation of a custom texture. Finish by callingTexture2DBuilder.Finish.
```c#
static TextureArrayBuilder CreateArray( int width = 1, int height = 1, int count = 1, ImageFormat format = 0) 
```
Begins creation of a custom texture array. Finish by callingTextureArrayBuilder.Finish.
```c#
static TextureCubeBuilder CreateCube( int width = 1, int height = 1, ImageFormat format = 0) 
```
Begins creation of a custom cube texture. (A texture with 6 sides) Finish by callingTextureCubeBuilder.Finish.
```c#
static TextureBuilder CreateCustom( ) 
```
Begins creation of a custom texture. Finish by callingTextureBuilder.Create.
```c#
static TextureBuilder CreateRenderTarget( ) 
```
Begins creation of arender target. Finish by callingTextureBuilder.Create.
Render targets can be used for fancy things likeGraphics.RenderToTexture.
```c#
static Texture CreateRenderTarget( string name, ImageFormat format, Vector2 size) 
```
A convenience function to quickly create arender target.
Render targets can be used for fancy things likeGraphics.RenderToTexture.
```c#
static Texture CreateRenderTarget( string name, ImageFormat format, Vector2 size, Texture oldTexture = null) 
```
This will create arender targettexture ifoldTextureis null or doesn't match what you've passed in. This is designed
to be called regularly to resize your texture in response to other things changing (like the screen size, panel size etc).
```c#
static Texture3DBuilder CreateVolume( int width, int height, int depth, ImageFormat format = 0) 
```
Begins creation of a custom 3D texture. Finish by callingTexture3DBuilder.Finish.
```c#
static Texture Find( string filepath) 
```
Try to get an already loaded texture.
```c#
static Texture Load( BaseFileSystem filesystem, string filepath, bool warnOnMissing = true) 
```
Try to load a texture from given filesystem, by filename.
```c#
static Texture Load( string url, bool warnOnMissing = true) 
```
Try to load a texture.
This version is able to load http images - but not images from disk.
```c#
static Task<Texture> LoadAsync( BaseFileSystem filesystem, string filepath, bool warnOnMissing = true) 
```
Load a texture asynchronously. Will return when the texture is loaded and valid.
This is useful when loading textures from the web.
```c#
static Texture LoadAvatar( long steamid) 
```
Load avatar image of a Steam user.
```c#
static Texture LoadAvatar( string steamid) 
```
Load avatar image of a Steam user.
```c#
virtual void Dispose( ) 
```
ImplementsIDisposable.DisposeWill release the handle for this texture. If the texture isn't referenced by anything
else it'll be released properly. This will happen anyway because it's called in the destructor.
By calling it manually you're just telling the engine you're done with this texture right now
instead of waiting for the garbage collector.
```c#
Color32 GetPixel( float x, float y, int mip = 0) 
```
Reads a single pixel color.
```c#
Color32 GetPixel3D( float x, float y, float z, int mip = 0) 
```
Reads a single pixel color from a volume or array texture.
```c#
Color32[] GetPixels( int mip = 0) 
```
Reads pixel colors from the texture at the specified mip level
```c#
void GetPixels<T,>( ValueTuple<int, int, int, int> srcRect, int slice, int mip, Span<T> dstData, ImageFormat dstFormat, ValueTuple<int, int> dstSize = null) 
```
Reads a 2D range of pixel values from the texture at the specified mip level, writing todstData.
This reads one slice from a 2D texture array or 3D texture volume.
```c#
void GetPixels3D<T,>( ValueTuple<int, int, int, int, int, int> srcBox, int mip, Span<T> dstData, ImageFormat dstFormat, ValueTuple<int, int, int> dstSize = null) 
```
Reads a 3D range of pixel values from the texture at the specified mip level, writing todstData.
This can be used with a 2D texture array, or a 3D volume texture.
```c#
void Update( ReadOnlySpan<byte> data, int x = 0, int y = 0, int width = 0, int height = 0) 
```
Update this texture with given raw data.
```c#
void Update( ReadOnlySpan<Color32> data, int x = 0, int y = 0, int width = 0, int height = 0) 
```
Update this texture with given raw data.
```c#
void Update( Color32 color, Rect rect) 
```
Write a coloured rectangle to the texture
```c#
void Update( Color32 color, float x, float y) 
```
Write a coloured pixel to the texture
```c#
void Update3D( ReadOnlySpan<byte> data, int x = 0, int y = 0, int z = 0, int width = 0, int height = 0, int depth = 0) 
```
Update this 3D texture with given raw data.
