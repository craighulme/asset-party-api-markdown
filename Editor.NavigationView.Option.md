# Option

## ```c#
Derives from Widget
```

## Summary

OverridesWidget.OnMousePressCalled when mouse is pressed over this widget.
## Constructors

```c#
Option( string title, string icon, NavigationView parent = null) 
```
No Summary
## Properties

```c#
Func<Widget> CreatePage { get; set; } 
```
No Summary
```c#
string Icon { get; set; } 
```
No Summary
```c#
bool IsSelected { get; set; } 
```
No Summary
```c#
Action OpenContextMenu { get; set; } 
```
No Summary
```c#
Widget Page { get; set; } 
```
No Summary
```c#
string Title { get; set; } 
```
No Summary
## Methods

```c#
Widget GetOrCreatePage( ) 
```
No Summary
```c#
protected override void OnMousePress( MouseEvent e) 
```
OverridesWidget.OnMousePressCalled when mouse is pressed over this widget.
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
