# FolderContextMenu

## 
```c#
Derives from ValueType
```

## Summary

Information about selected directory/folder when opening a context menu inEditor.AssetListor inEditor.AssetLocations.
## Fields

```c#
object Context
```
The panel that opened the context menu.Editor.AssetListor Editor.AssetFolderNode object.
```c#
Menu Menu
```
The menu to add context menu options to.
```c#
Vector2 ScreenPosition
```
Position of the cursor on screen when the context menu was opened.
```c#
DirectoryInfo Target
```
The folder we should be acting upon via context menu options.
```c#
bool ThisFolder
```
Clicked on empty space in a folder, not on a specific folder.
