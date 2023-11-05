# Paint

## ```c#
Derives from object
```

## Summary

Draws an arc (line). Angles are clockwise, 0 is north.
## Properties

```c#
static bool Antialiasing { set; } 
```
No Summary
```c#
static bool BilinearFiltering { set; } 
```
No Summary
```c#
static bool HasEnabled { get; } 
```
No Summary
```c#
static bool HasFocus { get; } 
```
No Summary
```c#
static bool HasMouseOver { get; } 
```
No Summary
```c#
static bool HasPressed { get; } 
```
No Summary
```c#
static bool HasSelected { get; } 
```
No Summary
```c#
static RenderMode RenderMode { set; } 
```
No Summary
```c#
static bool TextAntialiasing { set; } 
```
No Summary
## Methods

```c#
static void ClearBrush( ) 
```
No Summary
```c#
static void ClearPen( ) 
```
No Summary
```c#
static void Draw( Rect r, Pixmap pixmap, float alpha = 1) 
```
No Summary
```c#
static void Draw( Rect r, string image) 
```
No Summary
```c#
static void DrawArc( Vector2 center, Vector2 radius, float angle, float angleSize) 
```
Draws an arc (line). Angles are clockwise, 0 is north.
```c#
static void DrawArrow( Vector2 p1, Vector2 p2, float width) 
```
No Summary
```c#
static void DrawCircle( in Rect rect) 
```
No Summary
```c#
static void DrawCircle( Vector2 position, Vector2 scale) 
```
No Summary
```c#
static Rect DrawIcon( Rect rect, string iconName, float pixelHeight, TextFlag alignment = 132) 
```
No Summary
```c#
static void DrawLine( IEnumerable<Vector2> points) 
```
No Summary
```c#
static void DrawLine( in Vector2 from, in Vector2 to) 
```
No Summary
```c#
static void DrawPie( Vector2 center, Vector2 radius, float angle, float angleSize) 
```
Draws a pie. Angles are clockwise, 0 is north.
```c#
static void DrawPoints( IEnumerable<Vector2> points) 
```
No Summary
```c#
static void DrawPolygon( IEnumerable<Vector2> points) 
```
No Summary
```c#
static void DrawPolygon( Vector2[] points) 
```
No Summary
```c#
static void DrawRect( in Rect rect, float borderRadius) 
```
No Summary
```c#
static void DrawRect( in Rect rect) 
```
No Summary
```c#
static void DrawSquare( Vector2 position, Vector2 scale) 
```
No Summary
```c#
static Rect DrawText( in Vector2 position, string text) 
```
No Summary
```c#
static Rect DrawText( in Rect position, string text, TextFlag flags = 132) 
```
No Summary
```c#
static Rect DrawTextBox( Rect position, string text, Color textColor, Margin padding, float borderRadius, TextFlag flag) 
```
No Summary
```c#
static Pixmap LoadImage( string filename) 
```
No Summary
```c#
static Pixmap LoadImage( string filename, int x, int y) 
```
No Summary
```c#
static Rect MeasureText( in Rect position, string text, TextFlag flags = 132) 
```
No Summary
```c#
static Vector2 MeasureText( string text) 
```
No Summary
```c#
static void ResetTransform( ) 
```
No Summary
```c#
static void Rotate( float scale) 
```
No Summary
```c#
static void Rotate( float scale, Vector2 center) 
```
No Summary
```c#
static void Scale( float x, float y) 
```
No Summary
```c#
static void SetBrush( Color color) 
```
No Summary
```c#
static void SetBrush( string image) 
```
No Summary
```c#
static void SetBrush( Pixmap pixmap) 
```
No Summary
```c#
static void SetBrushEmpty( ) 
```
No Summary
```c#
static void SetBrushLinear( Vector2 a_pos, Vector2 b_pos, Color a_color, Color b_color) 
```
No Summary
```c#
static void SetBrushRadial( Vector2 center, float radius, Color a_color, Color b_color) 
```
No Summary
```c#
static void SetBrushRadial( Vector2 center, float radius, float a, Color a_color, float b, Color b_color) 
```
No Summary
```c#
static void SetDefaultFont( float size = 8, int weight = 400, bool italic = false, bool sizeInPixels = false) 
```
No Summary
```c#
static void SetFlags( bool selected, bool mouseOver, bool pressed, bool focused, bool enabled) 
```
No Summary
```c#
static void SetFont( string name, float size = 8, int weight = 400, bool italic = false, bool sizeInPixels = false) 
```
No Summary
```c#
static void SetPen( Color color, float size = 0, PenStyle style = 1) 
```
No Summary
```c#
static void SetPenEmpty( ) 
```
No Summary
```c#
static void Target( Pixmap pixmap) 
```
No Summary
```c#
static void Translate( Vector2 tx) 
```
No Summary
