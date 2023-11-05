# AssetVideo

## Derives from object

## Summary

Create the model or whatever
## Constructors

```c#
AssetVideo( Asset asset) 
```
No Summary
## Fields

```c#
SceneObject PrimarySceneObject
```
No Summary
```c#
Vector3 SceneCenter
```
No Summary
```c#
Vector3 SceneSize
```
No Summary
## Properties

```c#
Asset Asset { get; } 
```
No Summary
```c#
SceneCamera Camera { get; set; } 
```
No Summary
```c#
SceneWorld World { get; set; } 
```
No Summary
## Methods

```c#
static AssetVideo CreateForAsset( Asset asset) 
```
No Summary
```c#
static Pixmap RenderAssetThumbnail( Asset asset) 
```
No Summary
```c#
virtual void InitializeAsset( ) 
```
Create the model or whatever
```c#
virtual void InitializeScene( ) 
```
Create the world, camera, lighting
```c#
Task<byte[]> CreateVideo( float secondsLength, Config config) 
```
No Summary
```c#
void UpdateScene( float cycle, float timeStep) 
```
Cycle is a float 0-1, timestep is the time since the last frame
## Inheriting Types

