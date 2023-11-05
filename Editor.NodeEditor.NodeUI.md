# NodeUI

## ```c#
Derives from GraphicsItem
```

## Summary

OverridesGraphicsItem.OnMousePressed
## Constructors

```c#
NodeUI( GraphView graph, BaseNode node) 
```
No Summary
## Fields

```c#
protected bool _dragging
```
No Summary
```c#
List<PlugIn> Inputs
```
No Summary
```c#
List<PlugOut> Outputs
```
No Summary
```c#
Color PrimaryColor
```
No Summary
```c#
Color SelectionOutline
```
No Summary
## Properties

```c#
protected virtual float TitleHeight { get; } 
```
No Summary
```c#
DisplayInfo DisplayInfo { get; set; } 
```
No Summary
```c#
GraphView Graph { get; protected set; } 
```
No Summary
```c#
BaseNode Node { get; protected set; } 
```
No Summary
## Methods

```c#
protected virtual void Layout( ) 
```
No Summary
```c#
protected override void OnMousePressed( GraphicsMouseEvent e) 
```
OverridesGraphicsItem.OnMousePressed
```c#
protected override void OnMouseReleased( GraphicsMouseEvent e) 
```
OverridesGraphicsItem.OnMouseReleased
```c#
protected override void OnPaint( ) 
```
OverridesGraphicsItem.OnPaint
```c#
protected override void OnPositionChanged( ) 
```
OverridesGraphicsItem.OnPositionChanged
## Inheriting Types

