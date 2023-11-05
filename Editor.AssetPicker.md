# AssetPicker

## 
```c#
Derives from Dialog
```

## Summary

An asset browser allowing the user to pick a single asset.
Supports limiting display to only certain asset types.
## Constructors

```c#
AssetPicker( Widget parent, List<AssetType> assetTypes, bool showCloud = true) 
```
No Summary
```c#
AssetPicker( Widget parent, AssetType assetType, bool showCloud = true) 
```
No Summary
## Fields

```c#
bool MultiPick
```
Limited to 1 asset?
```c#
Button SaveButton
```
The button that picks the selected asset and closes the asset browser.
## Properties

```c#
AssetBrowser AssetBrowser { get; protected set; } 
```
Internal asset browser.
```c#
List<Asset> Assets { get; set; } 
```
The picked assets.
```c#
Action<Asset[]> OnAssetHighlighted { get; set; } 
```
Asset was highlighted, but not picked.
```c#
Action<Asset[]> OnAssetPicked { get; set; } 
```
An asset was picked. The asset picker will be closed after this.
## Methods

```c#
protected override void OnKeyPress( KeyEvent e) 
```
OverridesWidget.OnKeyPressA key has been pressed. Your widget needs keyboard focus for this to be called - see FocusMode.
