# PanelCreator

## Derives from ValueType

## Summary

Used forPanel.Addfor quick panel creation with certain settings. Other panels types are added via extension methods.
## Fields

```c#
Panel panel
```
The panel to add children to.
## Methods

```c#
Panel Panel( ) 
```
Add a new blank panel as a child.
```c#
Panel Panel( string classname) 
```
Add a new blank panel with given CSS classes as a child.
## Extensions

```c#
Button Button( string text, Action onClick = null) 
```
Create a button with given text and on-click action.
```c#
Button Button( string text, string className, Action onClick = null) 
```
Create a button with given text, CSS class name and on-click action.
```c#
ButtonGroup ButtonGroup( string classes = null) 
```
Creates a button group with given CSS classes.
```c#
Button ButtonWithConsoleCommand( string text, string command) 
```
Create a button with given text that runs a console command on click.
```c#
Button ButtonWithIcon( string text, string icon, string className, Action onClick = null) 
```
Create a button with given text, icon, CSS class name and on-click action.
```c#
IconPanel Icon( string icon, string classes = null) 
```
Create and return an icon (panel) with given icon and optionally given CSS classes.
```c#
Image Image( string image = null, string classname = null) 
```
Create an image with given texture and CSS classname.
```c#
Label Label( string text = null, string classname = null) 
```
Create a simple text label with given text and CSS classname.
```c#
ScenePanel ScenePanel( SceneWorld world, Vector3 position, Rotation rotation, float fieldOfView, string classname = null) 
```
No Summary
```c#
TextEntry TextEntry( string text = "") 
```
Creates and returns a text entry with predefined text already entered.
## Referencing Members

```c#
PanelCreator = Panel.Add { get; } 
```
```c#
static Button = ButtonConstructor.Button( PanelCreator, string, Action ) 
```
```c#
static Button = ButtonConstructor.Button( PanelCreator, string, string, Action ) 
```
```c#
static ButtonGroup = ButtonGroupConstructor.ButtonGroup( PanelCreator, string ) 
```
```c#
static Button = ButtonConstructor.ButtonWithConsoleCommand( PanelCreator, string, string ) 
```
```c#
static Button = ButtonConstructor.ButtonWithIcon( PanelCreator, string, string, string, Action ) 
```
```c#
static IconPanel = IconPanelConstructor.Icon( PanelCreator, string, string ) 
```
```c#
static Image = ImageConstructor.Image( PanelCreator, string, string ) 
```
```c#
static Label = LabelConstructor.Label( PanelCreator, string, string ) 
```
```c#
static ScenePanel = SceneConstructor.ScenePanel( PanelCreator, SceneWorld, Vector3, Rotation, float, string ) 
```
```c#
static TextEntry = TextEntryConstructor.TextEntry( PanelCreator, string ) 
```
