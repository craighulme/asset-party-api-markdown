# Rect

## Derives from ValueType
Implements IEquatable< Rect>

## Summary

Represents a rectangle.
## Constructors

```c#
Rect( float x, float y, float width, float height) 
```
Initialize a Rect at given position and with given size.
```c#
Rect( Vector2 point, Vector2 size = null) 
```
Initialize a Rect at given position and with given size.
## Properties

```c#
float Bottom { get; set; } 
```
Position of rect's bottom edge relative to its parent.
```c#
Vector2 BottomLeft { get; } 
```
Position of the bottom left edge of this rect.
```c#
Vector2 BottomRight { get; } 
```
Position of the bottom right edge of this rect.
```c#
Vector2 Center { get; } 
```
Center of this rect.
```c#
float Height { get; set; } 
```
Height of the rect.
```c#
float Left { get; set; } 
```
Position of rect's left edge relative to its parent, can also be interpreted as its position on the X axis.
```c#
Vector2 Position { get; set; } 
```
Position of this rect.
```c#
float Right { get; set; } 
```
Position of rect's right edge relative to its parent.
```c#
Vector2 Size { get; set; } 
```
Size of this rect.
```c#
float Top { get; set; } 
```
Position of rect's top edge relative to its parent, can also be interpreted as its position on the Y axis.
```c#
Vector2 TopLeft { get; } 
```
Position of the top left edge of this rect.
```c#
Vector2 TopRight { get; } 
```
Position of the top right edge of this rect.
```c#
float Width { get; set; } 
```
Width of the rect.
```c#
Rect WithoutPosition { get; } 
```
Returns this rect with position set to 0 on both axes.
## Methods

```c#
void Add( Rect r) 
```
Expand this Rect to contain the other rect
```c#
void Add( Vector2 point) 
```
Expand this Rect to contain the point
```c#
Rect AddPoint( Vector2 pos) 
```
Returns this rect expanded to include this point
```c#
Rect Align( in Vector2 size, TextFlag align) 
```
Align the smaller rect inside this rect.
Default alignment on each axis is Top, Left.
```c#
Rect Ceiling( ) 
```
Returns a Rect with position and size rounded up.
```c#
Rect Contain( in Vector2 size, TextFlag align = 132, bool stretch = false) 
```
Contain a given rectangle (image) within this rectangle (frame), preserving aspect ratio.
```c#
Rect Floor( ) 
```
Returns a Rect with position and size rounded down.
```c#
Rect Grow( float left, float top, float right, float bottom) 
```
Returns a Rect grown in every direction by given amounts.
```c#
Rect Grow( Margin m) 
```
Returns a Rect grown in every direction byMargin's values.
```c#
Rect Grow( float x, float y) 
```
Returns a Rect grown in every direction by given values on each axis.
```c#
Rect Grow( float amt) 
```
Returns a Rect grown in every direction by given amount.
```c#
bool IsInside( in Rect rect, bool fullyInside = false) 
```
Return true if the passed rect is partially or fully inside this rect.
```c#
bool IsInside( in Vector2 pos) 
```
Return true if the passed point is inside this rect.
```c#
Rect Round( ) 
```
Returns a Rect with position and size rounded to closest integer values.
```c#
Rect Shrink( float left, float top, float right, float bottom) 
```
Returns a Rect shrunk in every direction by given values.
```c#
Rect Shrink( Margin m) 
```
Returns a Rect shrunk in every direction byMargin's values.
```c#
Rect Shrink( float x, float y) 
```
Returns a Rect shrunk in every direction by given values on each axis.
```c#
Rect Shrink( float amt) 
```
Returns a Rect shrunk in every direction by given amount.
```c#
Vector4 ToVector4( ) 
```
Returns this rect as a Vector4, where X/Y/Z/W are Left/Top/Right/Bottom respectively.
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( Rect o) 
```
OverridesValueType.Equals
```c#
override int GetHashCode( ) 
```
OverridesValueType.GetHashCode
```c#
override string ToString( ) 
```
OverridesValueType.ToString
## Operators

```c#
Rect +( Rect r, Vector2 p) 
```
No Summary
```c#
Rect +( Rect a, Rect b) 
```
No Summary
```c#
bool ==( Rect left, Rect right) 
```
No Summary
```c#
bool !=( Rect left, Rect right) 
```
No Summary
```c#
Rect *( Rect a, float b) 
```
No Summary
```c#
Rect *( Rect a, Vector2 b) 
```
No Summary
## Referencing Members

```c#
AddOvalPathCommand.AddOvalPathCommand( Rect ) 
```
```c#
static void SandboxBaseExtensions.AddQuad( VertexBuffer, Rect ) 
```
```c#
AddRectPathCommand.AddRectPathCommand( Rect ) 
```
```c#
AddRoundRectPathCommand.AddRoundRectPathCommand( Rect, float, float ) 
```
```c#
Rect = SvgPath.Bounds { get; } 
```
```c#
Rect = BaseItemWidget.CanvasRect { get; } 
```
```c#
Rect = ChartBackground.ChartRect { get; } 
```
```c#
Rect = Box.ClipRect
```
```c#
void Widget.ConstrainTo( Rect ) 
```
```c#
Rect = Widget.ContentRect { get; } 
```
```c#
Rect = LineEdit.CursorRect { get; } 
```
```c#
static void Paint.Draw( Rect, Pixmap, float ) 
```
```c#
static void Paint.Draw( Rect, string ) 
```
```c#
static Rect = Graphics.DrawIcon( Rect, string, Color, float, TextFlag ) 
```
```c#
static Rect = Graphics.DrawIcon( Rect, string, Color, float, TextFlag ) 
```
```c#
static Rect = Paint.DrawIcon( Rect, string, float, TextFlag ) 
```
```c#
static Rect = Paint.DrawIcon( Rect, string, float, TextFlag ) 
```
```c#
static Rect = Graphics.DrawText( in Rect, string, Color, string, float, float, TextFlag ) 
```
```c#
static Rect = Graphics.DrawText( in Vector2, string, Color, string, float, float ) 
```
```c#
static Rect = Paint.DrawText( in Vector2, string ) 
```
```c#
static Rect = Paint.DrawText( in Rect, string, TextFlag ) 
```
```c#
static Rect = Paint.DrawTextBox( Rect, string, Color, Margin, float, TextFlag ) 
```
```c#
static Rect = Paint.DrawTextBox( Rect, string, Color, Margin, float, TextFlag ) 
```
```c#
IEnumerable<Panel> = Panel.FindInRect( Rect, bool ) 
```
```c#
Rect = Label.GetCaretRect( int ) 
```
```c#
Rect = GridLayout.GetCellRect( int, int ) 
```
```c#
Rect = TextEdit.GetCursorRect( TextCursor ) 
```
```c#
Rect = GridLayout.GetPosition( int ) 
```
```c#
static Pixmap = ProjectRow.GetProjectIcon( LocalProject, Rect ) 
```
```c#
abstract Rect = IPanel.InnerRect { get; } 
```
```c#
Rect = Layout.InnerRect { get; } 
```
```c#
bool = Panel.IsInside( Rect, bool ) 
```
```c#
Rect = GraphicsItem.LocalRect { get; } 
```
```c#
Rect = Widget.LocalRect { get; } 
```
```c#
Margin.Margin( Rect ) 
```
```c#
static Rect = Graphics.MeasureText( in Rect, string, string, float, float, TextFlag ) 
```
```c#
static Rect = Paint.MeasureText( in Rect, string, TextFlag ) 
```
```c#
virtual void BaseNode.OnPaint( Rect ) 
```
```c#
protected override void CloudProjectRow.OnPaintIcon( Rect ) 
```
```c#
protected virtual void ItemRow.OnPaintIcon( Rect ) 
```
```c#
protected override void ProjectRow.OnPaintIcon( Rect ) 
```
```c#
static Rect = RenderState.op_Implicit( RenderState ) 
```
```c#
void OrganisationProperty.OpenMenu( Rect ) 
```
```c#
abstract Rect = IPanel.OuterRect { get; } 
```
```c#
Rect = Layout.OuterRect { get; } 
```
```c#
static void GradientExtensions.PaintBlock( in Gradient, Rect ) 
```
```c#
protected virtual void ColorPicker.PaintHandle( Rect, float ) 
```
```c#
static void ColorPalette.PaintSwatch( Color, Rect, bool, float, bool ) 
```
```c#
Rect = RootPanel.PanelBounds { get; set; } 
```
```c#
Rect = SceneCamera.Rect { get; set; } 
```
```c#
abstract Rect = IPanel.Rect { get; } 
```
```c#
Rect = AddOvalPathCommand.Rect { get; init; } 
```
```c#
Rect = AddRectPathCommand.Rect { get; init; } 
```
```c#
Rect = AddRoundRectPathCommand.Rect { get; init; } 
```
```c#
Rect = Box.Rect
```
```c#
Rect = GridLayout.Rect { get; protected set; } 
```
```c#
Rect = VirtualWidget.Rect
```
```c#
Rect = Box.RectInner
```
```c#
Rect = Box.RectOuter
```
```c#
Rect = GraphicsView.SceneRect { get; set; } 
```
```c#
Rect = GraphicsItem.SceneRect { get; set; } 
```
```c#
Rect = Widget.ScreenGeometry { get; } 
```
```c#
Rect = Widget.ScreenRect { get; } 
```
```c#
void Pixmap.Scroll( int, int, Rect ) 
```
```c#
Rect = SelectionEvent.SelectionRect
```
```c#
Rect = GraphicsView.SelectionRect { set; } 
```
```c#
void PanelStyle.SetRect( Rect ) 
```
```c#
Action<Rect, float> = FloatSlider.SliderPaint { get; set; } 
```
```c#
void DebugOverlay.Texture( Texture, Rect, float ) 
```
```c#
void DebugOverlay.Texture( Texture, Rect, Color, Vector2, Vector2, float ) 
```
```c#
void Texture.Update( Color32, Rect ) 
```
```c#
protected virtual void RootPanel.UpdateBounds( Rect ) 
```
```c#
protected override void WorldPanel.UpdateBounds( Rect ) 
```
```c#
protected virtual void RootPanel.UpdateScale( Rect ) 
```
```c#
protected override void WorldPanel.UpdateScale( Rect ) 
```
```c#
static Rect = Graphics.Viewport { get; set; } 
```
