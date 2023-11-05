# WorldTextEntity

## ```c#
Derives from Entity
```

## Summary

3D text in the world
## Constructors

```c#
WorldTextEntity( ) 
```
No Summary
## Properties

```c#
Color Color { get; set; } 
```
No Summary
```c#
float DepthRenderOffset { get; set; } 
```
No Summary
```c#
string FontName { get; set; } 
```
No Summary
```c#
float FontSize { get; set; } 
```
No Summary
```c#
HorizontalJustify JustifyHorizontal { get; set; } 
```
No Summary
```c#
VerticalJustify JustifyVertical { get; set; } 
```
No Summary
```c#
string Message { get; set; } 
```
No Summary
```c#
float WorldUnitsPerPixel { get; set; } 
```
No Summary
## Methods

```c#
static void DrawGizmos( EditorContext context) 
```
No Summary
```c#
protected void OnFrame( ) 
```
No Summary
```c#
override void ClientSpawn( ) 
```
OverridesEntity.ClientSpawnCalled when the entity spawns on client.
```c#
protected override void OnDestroy( ) 
```
OverridesEntity.OnDestroyCalled when the entity was destroyed. This is not the same as the class destructor.
```c#
override void Spawn( ) 
```
OverridesEntity.SpawnCalled when the entity is spawned in. It should have all properties set by this point.
This is the place to set up your entity.
## Nested Types

