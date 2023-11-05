# Stage

## ```c#
Derives from Enum
```

## Summary

Describes a stage in the pipeline. The pipeline runs in this order:Render opaque sceneobjectsRender skybox sceneobjectsRender transparent sceneobjects (sorted)Render viewmodel (with adjusted znear/zfar)Render post processing effectsRender UI
## Fields

```c#
static Stage AfterOpaque = 10
```
No Summary
```c#
static Stage AfterPostProcess = 60
```
No Summary
```c#
static Stage AfterSkybox = 20
```
No Summary
```c#
static Stage AfterTransparent = 30
```
No Summary
```c#
static Stage AfterUI = 70
```
No Summary
```c#
static Stage AfterViewmodel = 40
```
No Summary
```c#
static Stage BeforePostProcess = 50
```
No Summary
## Referencing Members

```c#
virtual void RenderHook.OnStage( SceneCamera, Stage ) 
```
```c#
override void DepthOfField.OnStage( SceneCamera, Stage ) 
```
```c#
override void ScreenEffects.OnStage( SceneCamera, Stage ) 
```
