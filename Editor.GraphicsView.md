# GraphicsView

## Derives from Widget

## Summary

All items inside this rect will be selected
## Constructors

```c#
GraphicsView( Widget parent = null) 
```
No Summary
## Properties

```c#
bool Antialiasing { set; } 
```
No Summary
```c#
bool BilinearFiltering { set; } 
```
No Summary
```c#
ScrollbarMode HorizontalScrollbar { get; set; } 
```
No Summary
```c#
IEnumerable<GraphicsItem> Items { get; } 
```
No Summary
```c#
Action OnSelectionChanged { get; set; } 
```
No Summary
```c#
float Rotation { get; set; } 
```
No Summary
```c#
Vector2 Scale { get; set; } 
```
No Summary
```c#
Rect SceneRect { get; set; } 
```
No Summary
```c#
IEnumerable<GraphicsItem> SelectedItems { get; } 
```
No Summary
```c#
Rect SelectionRect { set; } 
```
All items inside this rect will be selected
```c#
bool TextAntialiasing { set; } 
```
No Summary
```c#
ViewportAnchorType TransformAnchor { get; set; } 
```
No Summary
```c#
ScrollbarMode VerticalScrollbar { get; set; } 
```
No Summary
## Methods

```c#
void Add( GraphicsItem t) 
```
No Summary
```c#
GraphicsWidget Add( Widget t) 
```
No Summary
```c#
void CenterOn( Vector2 center) 
```
No Summary
```c#
void DeleteAllItems( ) 
```
No Summary
```c#
Vector2 FromScene( Vector2 pos) 
```
No Summary
```c#
GraphicsItem GetItemAt( Vector2 scenePosition) 
```
No Summary
```c#
void SetBackgroundImage( string image) 
```
No Summary
```c#
void SetBackgroundImage( Pixmap image) 
```
No Summary
```c#
Vector2 ToScene( Vector2 pos) 
```
No Summary
```c#
void Translate( Vector2 delta) 
```
No Summary
```c#
void Zoom( float adjust, Vector2 viewpos) 
```
No Summary
## Nested Types

## Inheriting Types

