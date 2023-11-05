# HammerAssetBrowser

## ```c#
Derives from AssetBrowser
```

## Summary

Called when the selection set changes
## Constructors

```c#
HammerAssetBrowser( Widget parent) 
```
No Summary
## Properties

```c#
static HammerAssetBrowser Instance { get; } 
```
No Summary
## Methods

```c#
static protected void OnAssetContextMenu_Hammer( AssetContextMenu e) 
```
No Summary
```c#
void UpdateSelectedAssetList( ) 
```
Called when the selection set changes
```c#
override void UpdateAssetList( bool changes = false) 
```
OverridesAssetBrowser.UpdateAssetListUpdate the list of displayed assets.
