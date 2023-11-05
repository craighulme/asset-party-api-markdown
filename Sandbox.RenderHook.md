# RenderHook

## Is abstract
Derives from object

## Summary

A hook is added to a SceneCamera to allow you to add custom rendering effects within the pipeline.
## Constructors

```c#
protected RenderHook( ) 
```
No Summary
## Properties

```c#
bool Enabled { get; set; } 
```
Enable or disable this hook
```c#
int Order { get; set; } 
```
Lower values get called before others
## Methods

```c#
virtual void OnFrame( SceneCamera target) 
```
Called before the render to allow you to think. This is a good
place to do something like move sceneobjects.
```c#
virtual void OnStage( SceneCamera target, Stage renderStage) 
```
Called while rendering the scene. Check renderStage to find out where.
## Nested Types

## Inheriting Types

