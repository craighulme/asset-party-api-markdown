# NavLinkPanel

## 
```c#
Derives from Panel
```

## Summary

A panel that will navigate to an href but also have .active class if href is active
## Constructors

```c#
NavLinkPanel( ) 
```
No Summary
## Properties

```c#
string HRef { get; set; } 
```
No Summary
```c#
string Match { get; set; } 
```
No Summary
## Methods

```c#
protected override void OnClick( MousePanelEvent e) 
```
OverridesPanel.OnClickCalled when the player releases their left mouse button (Mouse 1) while hovering this panel.
```c#
override void OnParentChanged( ) 
```
OverridesPanel.OnParentChangedCalled after the parent of this panel has changed.
```c#
override void Tick( ) 
```
OverridesPanel.TickCalled every frame. This is your "Think" function.
