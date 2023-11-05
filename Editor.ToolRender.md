# ToolRender

## Is static
Derives from object

## Summary

Renders basic stuff for tool views
## Properties

```c#
static bool IsActiveView { get; } 
```
No Summary
## Methods

```c#
static void Draw2DCircle( Vector2 center, float radius, int segments, Color color) 
```
No Summary
```c#
static void Draw2DCross( Vector2 topLeft, Vector2 bottomRight, Color color) 
```
No Summary
```c#
static void Draw2DRectangleFilled( Vector2 topLeft, Vector2 bottomRight, Color color) 
```
No Summary
```c#
static void Draw2DRectangleOutlined( Vector2 topLeft, Vector2 bottomRight, Color color) 
```
No Summary
```c#
static void Draw2DRectangleTextured( Vector2 topLeft, Vector2 bottomRight, Texture texture, bool alpha = true, bool srgb = true) 
```
No Summary
```c#
static void DrawBox( Vector3 mins, Vector3 maxs, Color color) 
```
No Summary
```c#
static void DrawLine( Vector3 start, Vector3 end, Color startColor, Color endColor) 
```
No Summary
```c#
static void DrawLine( Vector3 start, Vector3 end, Color color) 
```
No Summary
```c#
static void DrawScreenText( string text, Vector2 pos, Color color) 
```
No Summary
```c#
static void DrawWorldSpaceText( string text, Vector3 pos, Vector2 pixelOffset2D, Color color, float minZoomLevelToRender) 
```
No Summary
