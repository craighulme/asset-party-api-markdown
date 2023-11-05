# Connection

## ```c#
Derives from GraphicsLine
```

## Summary

OverridesGraphicsItem.OnMouseMove
## Constructors

```c#
Connection( PlugOut output, PlugIn input) 
```
No Summary
```c#
Connection( PlugOut output) 
```
No Summary
## Properties

```c#
PlugIn Input { get; protected set; } 
```
No Summary
```c#
PlugOut Output { get; protected set; } 
```
No Summary
## Methods

```c#
void Disconnect( ) 
```
No Summary
```c#
void Layout( ) 
```
No Summary
```c#
protected override void OnMouseMove( GraphicsMouseEvent e) 
```
OverridesGraphicsItem.OnMouseMove
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
OverridesGraphicsLine.OnPaint
