# TextFlag

## ```c#
Derives from Enum
```

## Summary

Flags dictating position of text (and other elements).
Default alignment on each axis is Top, Left.
Values for each axis can be combined into a single value, conflicting values have undefined behavior.
## Fields

```c#
static TextFlag Absolute = 16
```
No Summary
```c#
static TextFlag Bottom = 64
```
Anchor to the bottom on the Y axis.
```c#
static TextFlag Center = 132
```
Align in the center on both axises.
```c#
static TextFlag CenterBottom = 68
```
Anchor to the bottom side, center horizontally.
```c#
static TextFlag CenterHorizontally = 4
```
Align in the center on the X axis.
```c#
static TextFlag CenterTop = 36
```
Anchor to the top side, center horizontally.
```c#
static TextFlag CenterVertically = 128
```
Align in the center on the Y axis.
```c#
static TextFlag DontClip = 512
```
Do not cutoff text beyond its bounds. Used inGraphics.DrawTextandGraphics.MeasureText.
```c#
static TextFlag Justify = 8
```
No Summary
```c#
static TextFlag Left = 1
```
Align to the left on the X axis.
```c#
static TextFlag LeftBottom = 65
```
Anchor to the bottom left corner.
```c#
static TextFlag LeftCenter = 129
```
Anchor to the left side, center vertically.
```c#
static TextFlag LeftTop = 33
```
Anchor to the top left corner.
```c#
static TextFlag Right = 2
```
Align to the right on the X axis.
```c#
static TextFlag RightBottom = 66
```
Anchor to the bottom right corner.
```c#
static TextFlag RightCenter = 130
```
Anchor to the right side, center vertically.
```c#
static TextFlag RightTop = 34
```
Anchor to the top right corner.
```c#
static TextFlag SingleLine = 256
```
Limit the text to a single line. Used inGraphics.DrawTextandGraphics.MeasureText.
```c#
static TextFlag Top = 32
```
Anchor to the top on the Y axis.
```c#
static TextFlag WordWrap = 4096
```
No Summary
```c#
static TextFlag WrapAnywhere = 8192
```
No Summary
## Referencing Members

```c#
T = GridLayout.AddCell<T,>( int, int, T, int, int, TextFlag ) 
```
```c#
Layout = GridLayout.AddCell( int, int, Layout, int, int, TextFlag ) 
```
```c#
Rect = Rect.Align( in Vector2, TextFlag ) 
```
```c#
TextFlag = Label.Alignment { get; set; } 
```
```c#
TextFlag = Layout.Alignment { get; set; } 
```
```c#
TextFlag = LineEdit.Alignment { get; set; } 
```
```c#
Rect = Rect.Contain( in Vector2, TextFlag, bool ) 
```
```c#
static Rect = Graphics.DrawIcon( Rect, string, Color, float, TextFlag ) 
```
```c#
static Rect = Paint.DrawIcon( Rect, string, float, TextFlag ) 
```
```c#
static Rect = Graphics.DrawText( in Rect, string, Color, string, float, float, TextFlag ) 
```
```c#
static Rect = Paint.DrawText( in Rect, string, TextFlag ) 
```
```c#
static Rect = Paint.DrawTextBox( Rect, string, Color, Margin, float, TextFlag ) 
```
```c#
static Rect = Graphics.MeasureText( in Rect, string, string, float, float, TextFlag ) 
```
```c#
static Rect = Paint.MeasureText( in Rect, string, TextFlag ) 
```
```c#
void GizmoDraw.ScreenText( string, Vector2, string, float, TextFlag ) 
```
```c#
abstract void IPanel.SetAbsolutePosition( TextFlag, Vector2, float ) 
```
```c#
void GizmoDraw.Text( string, Transform, string, float, TextFlag ) 
```
```c#
TextFlag = TextSceneObject.TextFlags { get; set; } 
```
```c#
void GizmoDraw.WorldText( string, Transform, string, float, TextFlag ) 
```
