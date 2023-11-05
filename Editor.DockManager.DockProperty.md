# DockProperty

## 
```c#
Derives from Enum
```

## Summary

When displaying this tool window in tabs, always display the tabs even if there's only one
## Fields

```c#
static DockProperty AlwaysDisplayFullTabs = 32
```
When displaying this tool window in tabs, always display the tabs even if there's only one
```c#
static DockProperty DisableDraggableTab = 4
```
Disable the user being able to drag this tab in the tab bar, to rearrange
```c#
static DockProperty DisallowFloatWindow = 16
```
Don't allow this tool window to be floated
```c#
static DockProperty DisallowUserDocking = 1
```
Disables all drag/docking ability by the user
```c#
static DockProperty HideCloseButton = 2
```
Hides the close button on the tab for this tool window
```c#
static DockProperty HideOnClose = 8
```
When the tool window is closed, hide it instead of removing it
## Referencing Members

```c#
void DockManager.AddDock( Widget, Widget, DockArea, DockProperty, float ) 
```
