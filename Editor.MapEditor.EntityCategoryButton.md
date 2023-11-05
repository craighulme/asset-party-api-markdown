# EntityCategoryButton

## Derives from Widget

## Summary

OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
## Constructors

```c#
EntityCategoryButton( Widget parent) 
```
No Summary
```c#
EntityCategoryButton( string text, Widget parent) 
```
No Summary
## Properties

```c#
string Icon { get; set; } 
```
No Summary
```c#
string MaterialIcon { get; set; } 
```
No Summary
```c#
bool Selected { get; set; } 
```
No Summary
```c#
string Text { get; set; } 
```
No Summary
## Methods

```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
```c#
override void Update( ) 
```
OverridesWidget.UpdateTell this widget that shit changed and it needs to redraw
