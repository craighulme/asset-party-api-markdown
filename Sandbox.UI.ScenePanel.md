# ScenePanel

## Derives from Panel

## Summary

Allows to render a scene world onto a panel.
## Constructors

```c#
ScenePanel( ) 
```
No Summary
## Properties

```c#
SceneCamera Camera { get; } 
```
The camera we're going to be using to render
```c#
bool RenderOnce { get; set; } 
```
If enabled, the scene will only render once. That isn't totally accurate though, because we'll
also re-render the scene when the size of the panel changes.
```c#
Texture RenderTexture { get; } 
```
The texture that the panel is rendering to internally. This will change to a different
texture if the panel changes size, so I wouldn't hold onto this object.
```c#
SceneWorld World { get; set; } 
```
Shortcut to Camera.World
```c#
override bool HasContent { get; } 
```
OverridesPanel.HasContentIf true, callsPanel.DrawContent.
## Methods

```c#
void RenderNextFrame( ) 
```
Render the panel again next frame. This is meant to be used with RenderOnce, where
you might want to render on demand or only once.
```c#
override void Delete( bool immediate = false) 
```
OverridesPanel.DeleteDeletes the panel.
```c#
override void SetProperty( string name, string value) 
```
OverridesPanel.SetPropertySet a property on the panel, such as special properties (class,id,styleandvalue, etc.) and properties of the panel's C# class.
