# EditorMainWindow

## Derives from DockWindow

## Summary

OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
## Properties

```c#
Menu FileMenu { get; init; } 
```
No Summary
```c#
Menu GameMenu { get; init; } 
```
No Summary
```c#
Menu ToolsMenu { get; init; } 
```
No Summary
```c#
Menu ViewsMenu { get; init; } 
```
No Summary
## Methods

```c#
void Frame( ) 
```
No Summary
```c#
void OnAssetSelected( Asset asset) 
```
No Summary
```c#
void SetVisible( bool visible) 
```
No Summary
```c#
void UpdateEditorTitle( string title) 
```
No Summary
```c#
protected override void DoLayout( ) 
```
OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
```c#
override void OnDestroyed( ) 
```
OverridesQObject.OnDestroyed
```c#
protected override void OnKeyPress( KeyEvent e) 
```
OverridesWidget.OnKeyPressA key has been pressed. Your widget needs keyboard focus for this to be called - see FocusMode.
```c#
protected override void RestoreDefaultDockLayout( ) 
```
OverridesDockWindow.RestoreDefaultDockLayoutOverride to apply a default layout to your window. This is called automatically from
RestoreFromStateCookie if there is no cookie set.
