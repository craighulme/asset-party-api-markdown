# SelectionDialog<T>

## Is abstract
Derives from PopupWidget

## Summary

A popup window that lets you select from a list.
Implement by:Override constructorSet window name, iconCall AddSearchHeader if you want the searchboxImplement OnSearchFilterFill BodyLayout with a ListView or ListTree etcSet SearchField.ForwardNavigationEvents if you want to forward navigation events to the listFire OnDoneClicked when double clicked an itemFire SelectItem to switch the currently selected item
## Type Parameters

```c#
T
```
No Summary
## Constructors

```c#
SelectionDialog( Widget parent = null) 
```
No Summary
## Properties

```c#
Layout BodyLayout { get; set; } 
```
Main layout
```c#
Button DoneButton { get; set; } 
```
The button used to accept the selection
```c#
Layout FooterLayout { get; set; } 
```
Footer with buttons
```c#
Layout HeaderLayout { get; set; } 
```
Header where the search box appears
```c#
Action<string> OnSearchFilter { get; set; } 
```
Called when search field text is modified
```c#
Action<T> OnSelectionChanged { get; set; } 
```
Called when selection is changed in the dialog
```c#
Action<T> OnSelectionFinished { get; set; } 
```
Called when the dialog is closed as a result of a successful selection
```c#
LineEdit SearchField { get; set; } 
```
Search field at the top of the page - created by calling AddSearchHeader
```c#
T Value { get; set; } 
```
The selected item.
## Methods

```c#
protected virtual void AddSearchHeader( ) 
```
Add the searchbox in the header. This is auto selected on open.
```c#
protected virtual void BuildFooter( ) 
```
Build the footer and create DoneButton (called in constructor)
```c#
protected virtual void OnSelectionComplete( ) 
```
Called when the done button is clicked and generally you should hook it up
so that double clicking an item calls this.
```c#
protected virtual void SelectItem( T value) 
```
Select the item and call OnSelectionChanged
