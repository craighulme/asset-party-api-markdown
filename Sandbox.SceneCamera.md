# SceneCamera

## Derives from object

## Summary

Represents a camera and holds render hooks. This camera can be used to draw tool windows and scene panels.
## Constructors

```c#
SceneCamera( string name = "Unnammed") 
```
No Summary
## Properties

```c#
Color AmbientLightColor { get; set; } 
```
No Summary
```c#
Angles Angles { get; set; } 
```
The rotation of the scene's camera.
```c#
bool AntiAliasing { get; set; } 
```
Enable or disable anti-aliasing for this render.
```c#
RenderAttributes Attributes { get; } 
```
No Summary
```c#
Color BackgroundColor { get; set; } 
```
Color the scene camera clears the render target to.
```c#
BloomAccessor Bloom { get; } 
```
Access tonemapping properties of camera
```c#
ClearFlags ClearFlags { get; set; } 
```
What kind of clearing should we do before we begin?
```c#
CubemapFogController CubemapFog { get; init; } 
```
Control fog based on an image.
```c#
bool EnablePostProcessing { get; set; } 
```
Toggle all post processing effects for this camera. The default is on.
```c#
bool EnableUserInterface { get; set; } 
```
Should we render the UI when rendering this camera
```c#
ITagSet ExcludeTags { get; } 
```
Scene objects with any of these tags won't be rendered by this camera.
```c#
float FieldOfView { get; set; } 
```
The horizontal field of view of the Camera in degrees.
```c#
IEntity FirstPersonViewer { get; set; } 
```
The entity that we're viewing from (if applicable)
```c#
bool IsMainCamera { get; } 
```
Returns true if this is the main game camera, on which game UI is drawn
```c#
string Name { get; set; } 
```
The name of this camera.. for debugging purposes.
```c#
Action OnRenderOpaque { get; set; } 
```
Called when rendering the transparent pass
```c#
Action OnRenderOverlay { get; set; } 
```
Called when rendering the camera's overlay
```c#
Action OnRenderPostProcess { get; set; } 
```
Called when rendering the transparent pass
```c#
Action OnRenderTransparent { get; set; } 
```
Called when rendering the transparent pass
```c#
bool Ortho { get; set; } 
```
Whether to use orthographic projection.
```c#
float OrthoHeight { get; set; } 
```
Height of the ortho whenSceneCamera.Orthois enabled.
```c#
float OrthoWidth { get; set; } 
```
Width of the ortho whenSceneCamera.Orthois enabled.
```c#
Vector3 Position { get; set; } 
```
The position of the scene's camera.
```c#
Rect Rect { get; set; } 
```
The rect of the screen to render to. This is normalized, between 0 and 1.
```c#
IEnumerable<RenderHook> RenderHooks { get; } 
```
List of active render hooks on this scene camera.
```c#
ITagSet RenderTags { get; } 
```
Only scene objects with one of these tags will be rendered by this camera.
```c#
Rotation Rotation { get; set; } 
```
The rotation of the scene's camera.
```c#
Vector2 Size { get; set; } 
```
The size of the screen. Allows us to work out aspect ratio.
For now will get updated automatically on render.
```c#
SkyboxAccessor Skybox { get; } 
```
Access skybox properties of camera
```c#
TonemapAccessor Tonemap { get; } 
```
Access tonemapping properties of camera
```c#
VolumetricFog VolumetricFog { get; init; } 
```
Control volumetric fog parameters, expect this to take 1-2ms of your GPU frame time.
```c#
SceneWorld World { get; set; } 
```
The world we're going to render.
```c#
HashSet<SceneWorld> Worlds { get; } 
```
Your camera can render multiple worlds.
```c#
float ZFar { get; set; } 
```
The camera's zFar distance. This is the furthest distance this camera will be able to render.
This value totally depends on the game you're making. Shorter the better, sensible ranges would be
between about 1000 and 30000, but if you want it to be further out you can balance that out by making
znear larger.
```c#
float ZNear { get; set; } 
```
The camera's zNear distance. This is the closest distance this camera will be able to render.
A good value for this is about 5. Below 5 and particularly below 1 you're going to start to see
a lot of artifacts like z-fighting.
## Methods

```c#
void AddHook( RenderHook value) 
```
Add a specific render hook to this camera.
```c#
T FindHook<T,>( ) 
```
Find a hook that matches the type, or null
```c#
RenderHook FindHook( Type t) 
```
Find a hook that matches the type, or null
```c#
T FindOrCreateHook<T,>( ) 
```
Find a hook that matches T, if not found then create and return
```c#
Ray GetRay( Vector3 cursorPosition) 
```
Given a cursor position get a scene aiming ray.
```c#
Ray GetRay( Vector3 cursorPosition, Vector3 screenSize) 
```
Given a cursor position get a scene aiming ray.
```c#
int RemoveAllHooks<T,>( ) 
```
Remove all hooks of type, return the amount of hooks removed
```c#
int RemoveAllHooks( ) 
```
Remove all hooks, return the amount removed
```c#
void RemoveHook( RenderHook value) 
```
Remove a specific render hook from this camera.
```c#
void SetViewModelCamera( float viewModelFieldOfView, float viewModelZNear = 1, float viewModelZFar = 500) 
```
Set attributes for rendering the viewmodel's camera.
```c#
Vector2 ToScreen( Vector3 world) 
```
Convert from world coords to screen coords. The results for x and y will be from 0 toSceneCamera.Size.
```c#
override string ToString( ) 
```
OverridesObject.ToString
## Extensions

```c#
bool RenderToPixmap( Pixmap targetPixmap, bool async = false) 
```
Render this camera to the target widget. Once you do this the target widget becomes "externally painted", so you
won't be able to paint on it anymore with Qt's Paint stuff.
```c#
bool RenderToVideo( VideoWriter videoWriter, TimeSpan? time = null) 
```
Render this camera to the target widget. Once you do this the target widget becomes "externally painted", so you
won't be able to paint on it anymore with Qt's Paint stuff.
```c#
Task<bool> RenderToVideoAsync( VideoWriter videoWriter, TimeSpan? time = null) 
```
Render this camera to the target widget. Once you do this the target widget becomes "externally painted", so you
won't be able to paint on it anymore with Qt's Paint stuff.
## Nested Types

