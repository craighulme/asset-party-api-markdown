# BasePage

## ```c#
Derives from Widget
```

## Summary

Rebuild the page on hotload for quick iteration
## Constructors

```c#
BasePage( ) 
```
No Summary
## Fields

```c#
Layout BodyLayout
```
No Summary
```c#
Layout Footer
```
No Summary
```c#
Layout FooterLeft
```
No Summary
```c#
Layout FooterRight
```
No Summary
```c#
Layout HeaderLayout
```
No Summary
## Properties

```c#
virtual string Icon { get; } 
```
No Summary
```c#
virtual LocalProject Project { get; } 
```
No Summary
```c#
virtual string Title { get; } 
```
No Summary
## Methods

```c#
virtual void InitFromProject( LocalProject project) 
```
No Summary
```c#
virtual void OnSave( ) 
```
No Summary
```c#
void AddFooterDefaults( ) 
```
No Summary
```c#
void Reset( ) 
```
Rebuild the page on hotload for quick iteration
```c#
Layout StartSection( string name, Layout layout = null) 
```
No Summary
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
## Inheriting Types

