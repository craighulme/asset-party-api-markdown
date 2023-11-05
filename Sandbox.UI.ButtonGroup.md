# ButtonGroup

## ```c#
Derives from Panel
```

## Summary

A group of side-by-side buttons one of which can be selected.
## Constructors

```c#
ButtonGroup( ) 
```
No Summary
## Properties

```c#
string ButtonClass { get; set; } 
```
CSS Class(es) to add to child buttons.
```c#
List<Option> Options { get; set; } 
```
Options to show in this button group.
```c#
Panel SelectedButton { get; set; } 
```
The selected button panel.
```c#
object Value { get; set; } 
```
The selected option value.
```c#
Action<string> ValueChanged { get; set; } 
```
Called when the value has been changed.
## Methods

```c#
Button AddButton( string value, Action action) 
```
Adds a button to this group.
```c#
Button AddButtonActive( string value, Action<bool> action) 
```
Adds a button to this button group withstartactiveandstopactivecallbacks
```c#
protected override void OnChildAdded( Panel child) 
```
OverridesPanel.OnChildAddedA child panel has been added to this panel.
```c#
protected override void OnParametersSet( ) 
```
OverridesPanel.OnParametersSetCalled after all templated panel binds have been set.
