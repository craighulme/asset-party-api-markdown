# ControlWidget

## Is abstract
Derives from Widget

## Summary

A control widget is used to edit the value of a single SerializedProperty.
## Constructors

```c#
ControlWidget( SerializedProperty property) 
```
No Summary
## Fields

```c#
static Color ControlColor
```
No Summary
```c#
static Color ControlHighlightPrimary
```
No Summary
```c#
static Color ControlHighlightSecondary
```
No Summary
```c#
static float ControlRadius
```
No Summary
```c#
static float ControlRowHeight
```
No Summary
```c#
bool PaintBackground
```
No Summary
## Properties

```c#
virtual bool IsControlActive { get; } 
```
No Summary
```c#
virtual bool IsControlButton { get; } 
```
No Summary
```c#
virtual bool IsControlDisabled { get; } 
```
No Summary
```c#
virtual bool IsControlHovered { get; } 
```
No Summary
```c#
virtual bool IsWideMode { get; } 
```
If true we prefer to be full inspector width
with the label above us
```c#
protected virtual int ValueHash { get; } 
```
No Summary
```c#
SerializedProperty SerializedProperty { get; } 
```
No Summary
## Methods

```c#
static ControlWidget Create( SerializedProperty property) 
```
No Summary
```c#
protected virtual void OnValueChanged( ) 
```
No Summary
```c#
protected virtual void PaintControl( ) 
```
No Summary
```c#
protected virtual void PaintOver( ) 
```
No Summary
```c#
protected virtual void PaintUnder( ) 
```
No Summary
```c#
virtual void Think( ) 
```
No Summary
```c#
protected override void OnContextMenu( ContextMenuEvent e) 
```
OverridesWidget.OnContextMenuCalled afterWidget.OnMouseRightClick, for the purposes of opening a context menu.
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

