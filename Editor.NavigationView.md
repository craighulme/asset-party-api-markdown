# NavigationView

## ```c#
Derives from Widget
```

## Summary

Bottom of the menu
## Constructors

```c#
NavigationView( Widget parent) 
```
No Summary
## Properties

```c#
Option CurrentOption { get; set; } 
```
No Summary
```c#
Widget CurrentPage { get; set; } 
```
No Summary
```c#
Layout MenuBottom { get; } 
```
Bottom of the menu
```c#
Layout MenuContents { get; } 
```
The menu
```c#
Layout MenuTop { get; } 
```
Top of the menu on the left
```c#
Layout PageContents { get; } 
```
The main content panel
## Methods

```c#
Option AddPage( string name, string icon, Widget page = null) 
```
No Summary
```c#
Option AddPage( DisplayInfo displayInfo, Widget page = null) 
```
No Summary
```c#
Option AddPage( Option tab) 
```
No Summary
```c#
void AddSectionHeader( string name) 
```
No Summary
```c#
void ClearPages( ) 
```
No Summary
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
## Nested Types

