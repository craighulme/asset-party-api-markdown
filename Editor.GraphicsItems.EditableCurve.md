# EditableCurve

## Derives from GraphicsItem

## Summary

Anatomy of an EditableCurve:
## Constructors

```c#
EditableCurve( GraphicsItem parent) 
```
No Summary
## Properties

```c#
Color CurveColor { get; set; } 
```
No Summary
```c#
float CurveThickness { get; set; } 
```
No Summary
```c#
float HandleDistance { get; set; } 
```
No Summary
```c#
List<Handle> Handles { get; } 
```
No Summary
```c#
Color SelectionColor { get; set; } 
```
No Summary
```c#
Vector2 TimeRange { get; } 
```
No Summary
```c#
Curve Value { get; set; } 
```
No Summary
```c#
Vector2 ValueRange { get; } 
```
No Summary
## Methods

```c#
virtual void HandleSelectionChanged( ) 
```
No Summary
```c#
void DeleteAllHandles( ) 
```
No Summary
```c#
void OnEdited( ) 
```
No Summary
```c#
void OnHandleMoved( ) 
```
No Summary
```c#
void SaveCurve( ) 
```
Write from editor to the curve (_value)
```c#
void UpdateTooltip( ) 
```
No Summary
```c#
override bool Contains( Vector2 localPos) 
```
OverridesGraphicsItem.Contains
```c#
protected override void OnMousePressed( GraphicsMouseEvent e) 
```
OverridesGraphicsItem.OnMousePressed
```c#
protected override void OnPaint( ) 
```
OverridesGraphicsItem.OnPaint
## Nested Types

