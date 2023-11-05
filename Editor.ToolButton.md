# ToolButton

## ```c#
Derives from Widget
```

## Summary

A button that shows as an icon and tries to keep itself square.
## Constructors

```c#
ToolButton( string name, string icon, Widget parent) 
```
No Summary
## Properties

```c#
bool Checked { get; set; } 
```
Whether the tool button is currently checked or not.
```c#
string Icon { get; set; } 
```
Icon for the tool button.
```c#
string IconChecked { get; set; } 
```
Icon to display when theToolButton.Checkedistrue.
```c#
bool IsToggle { get; set; } 
```
Whether the button is toggle-able or not.
## Methods

```c#
protected override void DoLayout( ) 
```
OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
```c#
protected override void OnMousePress( MouseEvent e) 
```
OverridesWidget.OnMousePressCalled when mouse is pressed over this widget.
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
