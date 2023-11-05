# DropDown

## Derives from PopupButton

## Summary

A UI control which provides multiple options via a dropdown box.
## Constructors

```c#
DropDown( ) 
```
No Summary
```c#
DropDown( Panel parent) 
```
No Summary
## Fields

```c#
protected IconPanel DropdownIndicator
```
The icon of an arrow pointing down on the right of the element.
## Properties

```c#
Func<List<Option>> BuildOptions { get; set; } 
```
Called just before opening, allows options to be dynamic
```c#
List<Option> Options { get; set; } 
```
The options to show on click. You can edit these directly via this property.
```c#
Option Selected { get; set; } 
```
The currently selected option.
```c#
object Value { get; set; } 
```
The current string value. This is useful to have if Selected is null.
```c#
Action<string> ValueChanged { get; set; } 
```
Called when the value has been changed,
## Methods

```c#
protected virtual void Select( Option option, bool triggerChange = true) 
```
Select an option.
```c#
protected virtual void Select( string value, bool triggerChange = true) 
```
Select an option by value string.
```c#
protected override void OnParametersSet( ) 
```
OverridesPanel.OnParametersSetCalled after all templated panel binds have been set.
```c#
override void Open( ) 
```
OverridesPopupButton.OpenOpen the dropdown.
```c#
override void SetPropertyObject( string name, object value) 
```
OverridesPanel.SetPropertyObjectSame asPanel.SetProperty, but first tries to set the property on the panel object, then process any special properties such asclass.
