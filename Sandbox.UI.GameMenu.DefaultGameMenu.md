# DefaultGameMenu

## Derives from NavHostPanel
Implements IGameMenuPanel

## Summary

OverridesPanel.BuildRenderTreeOverridden/implemented by Razor templating to build a render tree.
## Constructors

```c#
DefaultGameMenu( ) 
```
No Summary
## Methods

```c#
void OnLobbyJoined( ) 
```
No Summary
```c#
void OnLobbyLeave( ) 
```
No Summary
```c#
void OnServerJoined( ) 
```
No Summary
```c#
void OnServerLeave( ) 
```
No Summary
```c#
protected override void BuildRenderTree( RenderTreeBuilder __builder) 
```
OverridesPanel.BuildRenderTreeOverridden/implemented by Razor templating to build a render tree.
```c#
protected override string GetRenderTreeChecksum( ) 
```
OverridesPanel.GetRenderTreeChecksumOverridden/implemented by Razor templating, contains render tree checksum to determine when the render tree content has changed.
```c#
protected override void OnEvent( PanelEvent e) 
```
OverridesPanel.OnEventCalled when variousUI.PanelEvents happen. Handles event listeners and many standard events by default.
