# PopupButton

## 
```c#
Derives from Button
```

## Summary

A button that opens aPopupButton.Popuppanel.
Useless on its own - you need to implement Open
## Constructors

```c#
PopupButton( ) 
```
No Summary
## Fields

```c#
protected Popup Popup
```
The openedUI.Popup.
## Methods

```c#
abstract void Open( ) 
```
Open a popup. You should setPopupButton.Popuphere.
```c#
protected override void OnClick( MousePanelEvent e) 
```
OverridesPanel.OnClickCalled when the player releases their left mouse button (Mouse 1) while hovering this panel.
```c#
override void Tick( ) 
```
OverridesPanel.TickCalled every frame. This is your "Think" function.
## Inheriting Types

