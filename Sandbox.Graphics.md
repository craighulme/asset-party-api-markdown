# Graphics

## 
```c#
Derives from object
```

## Summary

Used to render to the screen using your Graphics Card, or whatever you
kids are using in your crazy future computers. Whatever it is I'm sure
it isn't fungible and everyone has free money and no-one has to ever work.
## Properties

```c#
static RenderAttributes Attributes { get; } 
```
Access to the current render context's attributes. These will be used
to set attributes in materials/shaders.
```c#
static bool IsActive { get; } 
```
If true then we're currently rendering and
you are safe to use the contents of this class
```c#
static SceneLayerType LayerType { get; } 
```
The current layer type. This is useful to tell whether you're meant to be drawing opaque, transparent or shadow. You mainly
don't need to think about this, but when you do, it's here.
```c#
static RenderTarget RenderTarget { get; set; } 
```
Get or set the current render target. Setting this will bind the render target and change the viewport to match it.
```c#
static Rect Viewport { get; set; } 
```
In pixel size, where are we rendering to?
## Methods

```c#
static void Blit( Material material, RenderAttributes attributes = null) 
```
Draw a screen space quad using the passed material. Your material should be using a
screenspace shader so it will actually render to the screen and not in worldspace at 0,0,0
```c#
static void Clear( Color color, bool clearColor = true, bool clearDepth = true, bool clearStencil = true) 
```
Clear the current drawing context to given color.
```c#
static void Clear( Color color, bool clearColor = true, bool clearDepth = true) 
```
No Summary
```c#
static void Clear( bool clearColor = true, bool clearDepth = true) 
```
Clear the current drawing context to given color.
```c#
static void Draw( Span<Vertex> vertices, int vertCount, Material material, RenderAttributes attributes = null, PrimitiveType primitiveType = 5) 
```
Draw a bunch of vertices
```c#
static void Draw( List<Vertex> vertices, int vertCount, Material material, RenderAttributes attributes = null, PrimitiveType primitiveType = 5) 
```
Draw a bunch of vertices
```c#
static void Draw( Span<Vertex> vertices, int vertCount, Span<UInt16> indices, int indexCount, Material material, RenderAttributes attributes = null, PrimitiveType primitiveType = 5) 
```
Draw a bunch of vertices
```c#
static Rect DrawIcon( Rect rect, string iconName, Color color, float fontSize = 20, TextFlag alignment = 132) 
```
Calls DrawText with "Material Icons" font. You can get a list of icons herehttps://fonts.google.com/icons?selected=Material+Icons
```c#
static void DrawQuad( in Rect rect, in Material material, in Color color, RenderAttributes attributes = null) 
```
Draw a quad in screenspace
```c#
static void DrawRoundedRectangle( in Rect rect, in Color color, in Vector4 cornerRadius = null, in Vector4 borderWidth = null, in Color borderColor = null) 
```
Draw a rounded rectangle, with optional border, in Material.UI.Box
```c#
static Rect DrawText( in Rect position, string text, Color color, string fontFamily = "Roboto", float fontSize = 20, float fontWeight = 450, TextFlag flags = 132) 
```
Draws a text quad in screenspace using the Material.UI.Text material.
```c#
static Rect DrawText( in Vector2 position, string text, Color color, string fontFamily = "Roboto", float fontSize = 20, float fontWeight = 450) 
```
Draws a text quad in screenspace using the Material.UI.Text material.
```c#
static void GenerateMipMaps( Texture texture, DownsampleMethod downsampleMethod = 0, int initialMip = 0, int numMips = -1) 
```
Generate the mip maps for this texture. Obviously the texture needs to support mip maps.
```c#
static void GenerateMipMaps( Texture texture) 
```
No Summary
```c#
static void GrabDepthTexture( string targetName, RenderAttributes renderAttributes, bool withMips) 
```
Grabs the current depth texture and stores it in 'targetName' on ''renderAttributes'
```c#
static void GrabDepthTexture( string targetName = "DepthTexture", RenderAttributes renderAttributes = null) 
```
TODO Painday: Remove
```c#
static void GrabFrameTexture( string targetName, RenderAttributes renderAttributes, bool withMips) 
```
Grabs the current viewport's color texture and stores it in 'targetName' on ''renderAttributes'
```c#
static void GrabFrameTexture( string targetName = "FrameTexture", RenderAttributes renderAttributes = null) 
```
TODO Painday: Remove
```c#
static Rect MeasureText( in Rect position, string text, string fontFamily = "Roboto", float fontSize = 20, float fontWeight = 450, TextFlag flags = 132) 
```
Measure how big some text will be, without having to render it
```c#
static void Render( SceneObject obj, Transform? transform = null, Color? color = null, Material material = null) 
```
Render a SceneObject
```c#
static bool RenderToTexture( SceneCamera camera, Texture target) 
```
Render this camera to the specified texture target
```c#
static void SetupLighting( SceneObject obj, RenderAttributes targetAttributes = null) 
```
Setup the lighting attributes for this current object. Place them in the targetAttributes
## Nested Types

