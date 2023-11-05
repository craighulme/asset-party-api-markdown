# GridLayout

## Derives from Layout

## Summary

A widget layout. You can think of it as an invisible box of rows or columns, each one containing a widget, useful for automatic positioning and scaling.
## Constructors

```c#
GridLayout( ) 
```
No Summary
## Properties

```c#
float HorizontalSpacing { get; set; } 
```
No Summary
```c#
float VerticalSpacing { get; set; } 
```
No Summary
## Methods

```c#
virtual T Add<T,>( T widget) 
```
No Summary
```c#
T AddCell<T,>( int x, int y, T widget, int xSpan = 1, int ySpan = 1, TextFlag alignment = 0) 
```
No Summary
```c#
Layout AddCell( int x, int y, Layout layout, int xSpan = 1, int ySpan = 1, TextFlag alignment = 0) 
```
No Summary
```c#
Rect GetCellRect( int x, int y) 
```
No Summary
```c#
void SetColumnStretch( float[] values) 
```
No Summary
```c#
void SetMinimumColumnWidth( int column, int width) 
```
No Summary
```c#
void SetMinimumRowHeight( int row, int height) 
```
No Summary
```c#
void SetRowStretch( float[] values) 
```
No Summary
```c#
override Layout Add( Layout layout) 
```
OverridesLayout.Add
```c#
override Layout Add( Layout layout, int stretch) 
```
OverridesLayout.Add
## Inheriting Types

