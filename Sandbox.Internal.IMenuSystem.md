# IMenuSystem

## Is interface

## Summary

This is how the engine communicates with the menu system
## Properties

```c#
abstract string Url { get; set; } 
```
The menu's current UI url
## Methods

```c#
abstract void CloseGameMenu( ) 
```
Close the currently active game menu, if there is one
```c#
abstract void Init( ) 
```
Called to initialize the menu system
```c#
abstract bool IsMenuScreenVisible( ) 
```
If the menu screen is open
```c#
abstract void Popup( string type, string title, string subtitle) 
```
Show a popup
```c#
abstract void SetMenuScreen( bool show) 
```
Show/Hide the menu screen
```c#
abstract void Shutdown( ) 
```
Close down the menu, delete everything
