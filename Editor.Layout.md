# Layout

## Is abstract
Derives from QObject

## Summary

An enabled layout adjusts dynamically to changes; a disabled layout acts as if it did not exist.
## Properties

```c#
TextFlag Alignment { get; set; } 
```
An enabled layout adjusts dynamically to changes; a disabled layout acts as if it did not exist.
```c#
bool Enabled { get; set; } 
```
An enabled layout adjusts dynamically to changes; a disabled layout acts as if it did not exist.
```c#
Rect InnerRect { get; } 
```
The rect of this layout excluding margins
```c#
Margin Margin { get; set; } 
```
The amount of space to leave free around the outside of the layout
```c#
Rect OuterRect { get; } 
```
The rect of this layout including margins
```c#
float Spacing { get; set; } 
```
The amount of space between items
## Methods

```c#
static Layout Column( bool reversed = false) 
```
No Summary
```c#
static Layout Flow( ) 
```
No Summary
```c#
static GridLayout Grid( ) 
```
No Summary
```c#
static Layout Row( bool reversed = false) 
```
No Summary
```c#
abstract Layout Add( Layout layout) 
```
No Summary
```c#
virtual Layout Add( Layout layout, int stretch) 
```
No Summary
```c#
virtual T Add<T,>( T widget) 
```
No Summary
```c#
virtual T Add<T,>( T widget, int stretch) 
```
No Summary
```c#
virtual void AddSpacingCell( float size) 
```
Add a spacing item
```c#
virtual void AddStretchCell( int stretch = 0) 
```
Add a stretch item
```c#
Layout AddColumn( int stretch = 0, bool reversed = false) 
```
No Summary
```c#
Layout AddFlow( int stretch = 0) 
```
No Summary
```c#
Layout AddRow( int stretch = 0, bool reversed = false) 
```
No Summary
```c#
Separator AddSeparator( bool light = false) 
```
Adds a 1 pixel line
```c#
void Clear( bool deleteWidgets) 
```
Remove all widgets from this layout, without deleting them outright.
## Inheriting Types

