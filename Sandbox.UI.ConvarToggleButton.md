# ConvarToggleButton

## Derives from Button

## Summary

A button that toggles a console variable between two given values.
## Constructors

```c#
ConvarToggleButton( ) 
```
No Summary
```c#
ConvarToggleButton( Panel parent, string label, string convar, string onvalue, string offvalue, string icon = null) 
```
No Summary
## Properties

```c#
string ConVar { get; set; } 
```
The console variable to modify using this button.
```c#
string ValueOff { get; set; } 
```
The "Off" value for the convar.
```c#
string ValueOn { get; set; } 
```
The "On" value for the convar, when the button is pressed in.
## Methods

```c#
void Toggle( ) 
```
Toggle the value of theConVarbetweenValueOnandValueOff.If the convar's value is not either one of those, it will be set toValueOn.
```c#
protected override void OnClick( MousePanelEvent e) 
```
OverridesPanel.OnClickCalled when the player releases their left mouse button (Mouse 1) while hovering this panel.
```c#
override void SetProperty( string name, string value) 
```
OverridesButton.SetPropertySet a property on the panel, such as special properties (class,id,styleandvalue, etc.) and properties of the panel's C# class.
```c#
override void Tick( ) 
```
OverridesPanel.TickCalled every frame. This is your "Think" function.
