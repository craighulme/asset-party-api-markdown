# Checkbox

## ```c#
Derives from Panel
```

## Summary

A simple checkboxUI.Panel.
## Constructors

```c#
Checkbox( ) 
```
No Summary
## Fields

```c#
protected bool isChecked
```
UseCheckbox.Checked.
PAINDAY TODO: Make private
## Properties

```c#
bool Checked { get; set; } 
```
Returns true if this checkbox is checked.
```c#
Panel CheckMark { get; protected set; } 
```
The checkmark icon. Although no guarantees it's an icon!
```c#
Label Label { get; protected set; } 
```
TheUI.Labelthat displaysCheckbox.LabelText.
```c#
string LabelText { get; set; } 
```
Text for the checkbox label.
```c#
bool Value { get; set; } 
```
Returns true if this checkbox is checked.
```c#
Action<bool> ValueChanged { get; set; } 
```
Called when the checked state has been changed.
## Methods

```c#
virtual void OnValueChanged( ) 
```
Called whenCheckbox.Valuechanges.
```c#
protected virtual void UpdateState( ) 
```
Called to update visuals of the checkbox. By default this appliescheckedCSS class.
```c#
protected override void OnClick( MousePanelEvent e) 
```
OverridesPanel.OnClickCalled when the player releases their left mouse button (Mouse 1) while hovering this panel.
```c#
protected override void OnMouseDown( MousePanelEvent e) 
```
OverridesPanel.OnMouseDownCalled when the player presses down the left or right mouse buttons while hovering this panel.
```c#
override void SetContent( string value) 
```
OverridesPanel.SetContentCalled by the templating system when an element has content between its tags.
```c#
override void SetProperty( string name, string value) 
```
OverridesPanel.SetPropertySet a property on the panel, such as special properties (class,id,styleandvalue, etc.) and properties of the panel's C# class.
