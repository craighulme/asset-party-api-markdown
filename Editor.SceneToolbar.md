# SceneToolbar

## ```c#
Derives from ToolBar
```

## Summary

A common toolbar which can be configured to control scene settings
## Constructors

```c#
SceneToolbar( Widget widget) 
```
No Summary
## Properties

```c#
Option GlobalSpace { get; } 
```
No Summary
```c#
Option PositionOption { get; } 
```
No Summary
```c#
Option RotationOption { get; } 
```
No Summary
```c#
Option ScaleOption { get; } 
```
No Summary
```c#
Instance SceneInstance { get; set; } 
```
No Summary
## Methods

```c#
virtual void AddAdvancedDropdown( ) 
```
No Summary
```c#
virtual void BuildToolbar( ) 
```
No Summary
```c#
virtual void OpenCameraDropdown( ) 
```
No Summary
```c#
virtual void OpenDropdown( ) 
```
No Summary
```c#
void AddCameraDropdown( ) 
```
No Summary
```c#
void AddGizmoModes( ) 
```
Add position, rotation, scale
```c#
void BuildDefault( Instance sceneInstance) 
```
No Summary
```c#
void SwitchMode( string controlMode) 
```
Switch control mode to this mode (usually position, rotation, scale)
