# ButtonConstructor

## ```c#
Derives from object
```

## Summary

Create a button with given text and on-click action.
## Methods

```c#
static Button Button( PanelCreator self, string text, Action onClick = null) 
```
Create a button with given text and on-click action.
```c#
static Button Button( PanelCreator self, string text, string className, Action onClick = null) 
```
Create a button with given text, CSS class name and on-click action.
```c#
static Button ButtonWithConsoleCommand( PanelCreator self, string text, string command) 
```
Create a button with given text that runs a console command on click.
```c#
static Button ButtonWithIcon( PanelCreator self, string text, string icon, string className, Action onClick = null) 
```
Create a button with given text, icon, CSS class name and on-click action.
