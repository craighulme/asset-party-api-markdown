# IAssetEditor

## Is interface

## Summary

A widget (usually window) implementing this will be able to edit assets via the asset browser.
The widget should be marked with the attribute of the asset's extension, like this[CanEdit( "asset:vsndstck" )]
## Fields

```c#
static Dictionary<string, Widget> OpenEditors
```
A list of open editors for each asset type.
## Properties

```c#
abstract bool CanOpenMultipleAssets { get; } 
```
If this editor is able to edit multiple assets at the same time then return true
and we'll try to create only one version of that editor and AssetOpen will be called multiple times.
## Methods

```c#
static bool OpenInEditor( Asset asset) 
```
Open given asset in a new asset editor window. Will reuse already open editors for same asset type if the editor supports it. (IAssetEditor.CanOpenMultipleAssets)
```c#
static bool TryOpenUsingStaticMethod( Asset asset) 
```
No Summary
```c#
abstract void AssetOpen( Asset asset) 
```
Open the asset in this editor.
