# Hammer

## 
```c#
Derives from object
```

## Summary

The active editor session's map document.
## Properties

```c#
static MapDocument ActiveMap { get; } 
```
The active editor session's map document.
```c#
static Material CurrentMaterial { get; } 
```
Current Material - you can set this programmatically withHammer.SetCurrentMaterial
```c#
static Asset MapAsset { get; } 
```
No Summary
```c#
static bool Open { get; } 
```
If the Hammer app has been opened.
```c#
static Window Window { get; } 
```
The Hammer app's window.
## Methods

```c#
static void AssignAssetToSelection( Asset asset) 
```
Assigns the asset to the current selection.
```c#
static void ReloadFromFile( ) 
```
Reloads the active editor session from file with user prompt
```c#
static void SelectFacesUsingMaterial( Asset asset) 
```
Selects all faces using the asset, forcesSelection.SelectModetoSelectMode.Faces
```c#
static void SelectObjectsUsingAsset( Asset asset) 
```
Selects all map nodes using the asset, appending them to the current selection.
```c#
static void SetCurrentMaterial( Asset asset) 
```
Sets the currently used material to the specified asset.
```c#
static void ShowEntityReportForAsset( Asset asset) 
```
Opens a Entity Report dialog showing all entities using this asset.
