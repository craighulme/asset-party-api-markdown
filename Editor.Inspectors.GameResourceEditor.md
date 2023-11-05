# GameResourceEditor

## 
```c#
Implements IAssetEditor
```

## Summary

ImplementsIAssetEditor.CanOpenMultipleAssetsIf this editor is able to edit multiple assets at the same time then return true
and we'll try to create only one version of that editor and AssetOpen will be called multiple times.
## Constructors

```c#
GameResourceEditor( ) 
```
No Summary
## Properties

```c#
virtual bool CanOpenMultipleAssets { get; } 
```
ImplementsIAssetEditor.CanOpenMultipleAssetsIf this editor is able to edit multiple assets at the same time then return true
and we'll try to create only one version of that editor and AssetOpen will be called multiple times.
## Methods

```c#
virtual void AssetOpen( Asset asset) 
```
ImplementsIAssetEditor.AssetOpenOpen the asset in this editor.
