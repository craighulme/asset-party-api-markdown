# Dialog

## Derives from Widget

## Summary

A wrapper to more easily create dialog windows.
## Constructors

```c#
Dialog( Widget parent = null, bool initAsDialog = true) 
```
No Summary
## Properties

```c#
Window Window { get; init; } 
```
The created parent window for this dialog.
## Methods

```c#
static void AskConfirm( Action OnSuccess, string question, string title = "Confirmation", string okay = "Okay", string cancel = "Cancel") 
```
Ask for a confirmation
```c#
static void AskString( Action<string> OnSuccess, string question, string okay = "Okay", string cancel = "Cancel", string initialName = "", string title = "Input required") 
```
Ask for a string
```c#
static void AskStringFile( Action<string> OnSuccess, string question, string okay = "Okay", string cancel = "Cancel", string initialName = "") 
```
Ask for a string which is intended to be a new file name.. which means it shouldn't have / or " or : etc.
```c#
static void AskStringFolder( Action<string> OnSuccess, string question, string okay = "Okay", string cancel = "Cancel", string initialName = "") 
```
Ask for a string which is intended to be a new folder name.. which means it shouldn't have / or " or : etc.
```c#
override void Close( ) 
```
OverridesWidget.CloseIf a window - will close
```c#
override void Hide( ) 
```
OverridesWidget.HideMake this widget not visible.
```c#
override void Show( ) 
```
OverridesWidget.ShowMake this widget visible.
## Inheriting Types

