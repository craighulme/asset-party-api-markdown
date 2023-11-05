# Window

## 
```c#
Derives from DockWindow
```

## Summary

OverridesWindow.OnClosedCalled when a window is closed.
## Constructors

```c#
Window( ) 
```
No Summary
## Properties

```c#
bool CanOpenMultipleAssets { get; } 
```
No Summary
## Methods

```c#
static void OnModelDocToolsMenu( Menu menu) 
```
No Summary
```c#
void AssetOpen( Asset asset) 
```
No Summary
```c#
void CreateUI( ) 
```
No Summary
```c#
void OnHotload( ) 
```
No Summary
```c#
protected override void OnClosed( ) 
```
OverridesWindow.OnClosedCalled when a window is closed.
```c#
protected override void RestoreDefaultDockLayout( ) 
```
OverridesDockWindow.RestoreDefaultDockLayoutOverride to apply a default layout to your window. This is called automatically from
RestoreFromStateCookie if there is no cookie set.
