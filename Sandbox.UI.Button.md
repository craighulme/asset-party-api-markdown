# Button

## 
```c#
Derives from Panel
```

## Summary

A simple buttonUI.Panel.
## Constructors

```c#
Button( ) 
```
No Summary
```c#
Button( string text) 
```
No Summary
```c#
Button( string text, string icon) 
```
No Summary
```c#
Button( string text, string icon, Action onClick) 
```
No Summary
## Fields

```c#
protected IconPanel IconPanel
```
TheButton.IconPanelthat displaysButton.Icon.
```c#
protected Label TextLabel
```
TheUI.Labelthat displaysButton.Text.
## Properties

```c#
string Icon { get; set; } 
```
Icon for the button.
```c#
string Text { get; set; } 
```
Text for the button.
## Methods

```c#
virtual void SetText( string text) 
```
Set the text for the button. CallsText = value
```c#
void Click( ) 
```
Imitate the button being clicked.
```c#
void DeleteIcon( ) 
```
Deletes theButton.Icon.
```c#
void DeleteText( ) 
```
Deletes theButton.Text.
```c#
override void SetContent( string value) 
```
OverridesPanel.SetContentCalled by the templating system when an element has content between its tags.
```c#
override void SetProperty( string name, string value) 
```
OverridesPanel.SetPropertySet a property on the panel, such as special properties (class,id,styleandvalue, etc.) and properties of the panel's C# class.
## Inheriting Types

