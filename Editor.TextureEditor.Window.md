# Window

## 
```c#
Implements IAssetEditor
```

## Summary

ImplementsIAssetEditor.CanOpenMultipleAssetsIf this editor is able to edit multiple assets at the same time then return true
and we'll try to create only one version of that editor and AssetOpen will be called multiple times.
## Constructors

```c#
Window( ) 
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
```c#
void BuildMenuBar( ) 
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
protected override bool OnClose( ) 
```
OverridesWidget.OnCloseCalled when a window is about to be closed.
```c#
protected override void RestoreDefaultDockLayout( ) 
```
OverridesDockWindow.RestoreDefaultDockLayoutOverride to apply a default layout to your window. This is called automatically from
RestoreFromStateCookie if there is no cookie set.
