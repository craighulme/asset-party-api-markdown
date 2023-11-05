# Sky

## Derives from Entity

## Summary

Controls the sky.
## Constructors

```c#
Sky( ) 
```
No Summary
## Properties

```c#
float FogMaxEnd { get; set; } 
```
No Summary
```c#
float FogMaxStart { get; set; } 
```
No Summary
```c#
float FogMinEnd { get; set; } 
```
No Summary
```c#
float FogMinStart { get; set; } 
```
No Summary
```c#
FogType FogType { get; set; } 
```
No Summary
```c#
Material SkyMaterial { get; set; } 
```
No Summary
```c#
string Skyname { get; set; } 
```
No Summary
```c#
SceneSkyBox SkyObject { get; set; } 
```
No Summary
```c#
Color TintColor { get; set; } 
```
Tint the skybox
## Methods

```c#
override void ClientSpawn( ) 
```
OverridesEntity.ClientSpawnCalled when the entity spawns on client.
