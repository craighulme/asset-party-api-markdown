# ItemRow

## ```c#
Derives from Widget
```

## Summary

OverridesWidget.OnMouseClickCalled when this widget is left clicked (on mouse release).
## Constructors

```c#
ItemRow( Widget parent = null) 
```
No Summary
## Fields

```c#
static protected float TargetHeight
```
No Summary
## Properties

```c#
Action Click { get; set; } 
```
No Summary
```c#
bool IsActive { get; set; } 
```
No Summary
```c#
string Title { get; set; } 
```
No Summary
## Methods

```c#
static ItemRow From<T,>( T item, Widget parent = null) 
```
No Summary
```c#
protected virtual void CreateUI( ) 
```
No Summary
```c#
protected virtual List<InfoItem> GetInfo( ) 
```
No Summary
```c#
protected virtual void Init( ) 
```
No Summary
```c#
protected virtual bool IsDisabled( ) 
```
No Summary
```c#
virtual void OnClick( ) 
```
No Summary
```c#
protected virtual void OnPaintIcon( Rect iconRect) 
```
No Summary
```c#
IconButton AddButton( string icon, string tooltip, Action onClick = null) 
```
No Summary
```c#
protected override void OnMouseClick( MouseEvent e) 
```
OverridesWidget.OnMouseClickCalled when this widget is left clicked (on mouse release).
```c#
protected override void OnPaint( ) 
```
OverridesWidget.OnPaintOverride to custom paint your widget, for example usingEditor.Paint. Can be overwritten byWidget.OnPaintOverride.
```c#
protected override Vector2 SizeHint( ) 
```
OverridesWidget.SizeHintShould return the size this widget really wants to be if it can its way. The default
is that you don't care - and just to return whatever the base value is.
## Inheriting Types

