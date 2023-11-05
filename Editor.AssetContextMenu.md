# AssetContextMenu

## 
```c#
Derives from ValueType
```

## Summary

Information about selected asset(s) when opening a context menu inEditor.AssetList.
## Fields

```c#
AssetList AssetList
```
The panel that opened the context menu.
```c#
Menu Menu
```
The menu to add context menu options to.
```c#
Vector2 ScreenPosition
```
Position of the cursor on screen when the context menu was opened.
```c#
List<Asset> SelectedList
```
List of selected assets when the context menu was opened.
These are the assets context menu should be affecting.
## Referencing Members

```c#
static protected void HammerAssetBrowser.OnAssetContextMenu_Hammer( AssetContextMenu ) 
```
