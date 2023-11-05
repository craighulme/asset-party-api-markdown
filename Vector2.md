# Vector2

## 
```c#
Implements IEquatable<Vector2>, IParsable<Vector2>
```

## Summary

A 2-dimensional vector. Typically represents a position or size in 2D space.
## Constructors

```c#
Vector2( float x, float y) 
```
Initializes a 2D vector with given components.
```c#
Vector2( float all) 
```
Initializes the vector with all components set to the given value.
```c#
Vector2( Vector3 v) 
```
Initializes the 2D vector with components from given 3D vector, discarding the Z component.
```c#
Vector2( Vector2 v) 
```
No Summary
## Fields

```c#
static readonly Vector2 Down
```
Returns a 2D vector with Y set to -1. This represents the downwards direction in 2D space.
```c#
static readonly Vector2 Left
```
Returns a 2D vector with X set to 1. This represents the left hand direction in 2D space.
```c#
static readonly Vector2 One
```
Returns a 2D vector with every component set to 1
```c#
static readonly Vector2 Right
```
Returns a 2D vector with X set to -1. This represents the right hand direction in 2D space.
```c#
static readonly Vector2 Up
```
Returns a 2D vector with Y set to 1. This represents the upwards direction in 2D space.
```c#
static readonly Vector2 Zero
```
Returns a 2D vector with every component set to 0
## Properties

```c#
static Vector2 Random { get; } 
```
Uniformly samples a 2D position from all points with distance at most 1 from the origin.
```c#
float Degrees { get; } 
```
Return the angle of this vector in degrees, always between 0 and 360
```c#
bool IsNearZeroLength { get; } 
```
Returns true if the squared length is less than 1e-8 (which is really near zero)
```c#
float Length { get; } 
```
Returns the magnitude of the vector
```c#
float LengthSquared { get; } 
```
This is faster than Length, so is better to use in certain circumstances
```c#
Vector2 Normal { get; } 
```
Return the same vector but with a length of one
```c#
Vector2 Perpendicular { get; } 
```
Returns a vector that runs perpendicular to this one
```c#
float x { get; set; } 
```
X component of this Vector.
```c#
float y { get; set; } 
```
Y component of this Vector.
## Methods

```c#
static float Distance( in Vector2 a, in Vector2 b) 
```
Returns distance between the 2 given vectors.
```c#
static float DistanceBetween( Vector2 a, Vector2 b) 
```
Returns distance between the 2 given vectors.
```c#
static float DistanceBetweenSquared( Vector2 a, Vector2 b) 
```
Returns squared distance between the 2 given vectors. This is faster thanDistanceBetween,
and can be used for things like comparing distances, as long as only squared values are used.
```c#
static float DistanceSquared( in Vector2 a, in Vector2 b) 
```
Returns squared distance between the 2 given vectors. This is faster thanDistanceBetween,
and can be used for things like comparing distances, as long as only squared values are used.
```c#
static float Dot( Vector2 a, Vector2 b) 
```
Returns dot product between the 2 given vectors.
```c#
static Vector2 FromDegrees( float degrees) 
```
Returns a point on a circle at given rotation from X axis, counter clockwise.
```c#
static Vector2 FromRadians( float radians) 
```
Returns a point on a circle at given rotation from X axis, counter clockwise.
```c#
static Vector2 Lerp( Vector2 a, Vector2 b, float t, bool clamp = true) 
```
Linearly interpolate from point a to point b.
```c#
static Vector2 Lerp( Vector2 a, Vector2 b, Vector2 t, bool clamp = true) 
```
Linearly interpolate from point a to point b with separate fraction for each axis.
```c#
static Vector2 Max( Vector2 a, Vector2 b) 
```
Returns a vector that has the maximum values on each axis between the 2 given vectors.
```c#
static Vector2 Min( Vector2 a, Vector2 b) 
```
Returns a vector that has the minimum values on each axis between the 2 given vectors.
```c#
static Vector2 Parse( string str) 
```
Given a string, try to convert this into a vector4. Example formatting is "x,y", "[x,y]", "x y", etc.
```c#
static Vector2 Parse( string str, IFormatProvider provider) 
```
ImplementsIParsable`1.ParseGiven a string, try to convert this into a vector4. Example formatting is "x,y", "[x,y]", "x y", etc.
```c#
static Vector2 Read( BinaryReader reader) 
```
Read a vector2 from given binary reader.
```c#
static bool TryParse( string str, out Vector2 result) 
```
Given a string, try to convert this into a vector4. Example formatting is "x,y", "[x,y]", "x y", etc.
```c#
static bool TryParse( string str, IFormatProvider provider, out Vector2 result) 
```
ImplementsIParsable`1.TryParseGiven a string, try to convert this into a vector4. Example formatting is "x,y", "[x,y]", "x y", etc.
```c#
Vector2 Abs( ) 
```
Returns a new vector with all values positive. -5 becomes 5, etc.
```c#
bool AlmostEqual( Vector2 v, float delta = 0.0001) 
```
Returns true if we're nearly equal to the passed vector.
```c#
Vector2 Clamp( Vector2 otherMin, Vector2 otherMax) 
```
Returns a vector each axis of which is clamped to between the 2 given vectors. Basically clamps a point to a square.
```c#
Vector2 Clamp( float min, float max) 
```
Returns a vector each axis of which is clamped to given min and max values.
```c#
Vector2 ComponentMax( Vector2 other) 
```
Returns a vector that has the maximum values on each axis between this vector and given vector.
```c#
Vector2 ComponentMin( Vector2 other) 
```
Returns a vector that has the minimum values on each axis between this vector and given vector.
```c#
float Distance( Vector2 target) 
```
Returns distance between this and given vectors.
```c#
float DistanceSquared( Vector2 target) 
```
Returns squared distance between the 2 given vectors. This is faster thanDistance,
and can be used for things like comparing distances, as long as only squared values are used.
```c#
Vector2 LerpTo( Vector2 target, float t, bool clamp = true) 
```
Linearly interpolate from this vector to given vector.
```c#
Vector2 LerpTo( Vector2 target, Vector2 t, bool clamp = true) 
```
Linearly interpolate from this vector to given vector with separate fraction for each axis.
```c#
Vector2 SnapToGrid( float gridSize, bool sx = true, bool sy = true) 
```
Snap to grid along all 3 axes.
```c#
Vector2 WithX( float x) 
```
Return this vector with given X.
```c#
Vector2 WithY( float y) 
```
Return this vector with given Y.
```c#
void Write( BinaryWriter writer) 
```
Write this vector2 to a System.IO.BinaryWriter.
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( Vector2 o) 
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
Vector2 +( Vector2 c1, Vector2 c2) 
```
No Summary
```c#
Vector2 /( Vector2 c1, Vector2 c2) 
```
No Summary
```c#
Vector2 /( Vector2 c1, float c2) 
```
No Summary
```c#
bool ==( Vector2 left, Vector2 right) 
```
No Summary
```c#
bool !=( Vector2 left, Vector2 right) 
```
No Summary
```c#
Vector2 *( Vector2 c1, float f) 
```
No Summary
```c#
Vector2 *( float f, Vector2 c1) 
```
No Summary
```c#
Vector2 *( Vector2 c1, Vector2 c2) 
```
No Summary
```c#
Vector2 -( Vector2 c1, Vector2 c2) 
```
No Summary
```c#
Vector2 -( Vector2 c1) 
```
No Summary
```c#
implicit Vector2 =( Vector2 value) 
```
No Summary
```c#
implicit Vector2 =( Vector2 value) 
```
No Summary
```c#
implicit Vector2 =( Vector3 value) 
```
No Summary
```c#
implicit Vector4 =( Vector2 value) 
```
No Summary
```c#
implicit Vector2 =( double value) 
```
No Summary
## Referencing Members

```c#
protected Vector2 = Slider2D._value
```
```c#
void Rect.Add( Vector2 ) 
```
```c#
static void SandboxBaseExtensions.Add( VertexBuffer, Vector3, Vector2 ) 
```
```c#
Rect = Rect.AddPoint( Vector2 ) 
```
```c#
AddPolyPathCommand.AddPolyPathCommand( IReadOnlyList<Vector2>, bool ) 
```
```c#
void WaterRipple.AddRipple( Vector2, Vector2, float, float ) 
```
```c#
void GlassShard.AddVertex( Vector2 ) 
```
```c#
virtual IAsyncResult = TextureChangedDelegate.BeginInvoke( ReadOnlySpan<byte>, Vector2, AsyncCallback, object ) 
```
```c#
virtual IAsyncResult = TextureChangedDelegate.BeginInvoke( ReadOnlySpan<byte>, Vector2, AsyncCallback, object ) 
```
```c#
Vector2 = Rect.BottomLeft { get; } 
```
```c#
Vector2 = Rect.BottomRight { get; } 
```
```c#
void GraphView.BuildFromNodes( IEnumerable<BaseNode>, Vector2, bool ) 
```
```c#
Matrix = PanelTransform.BuildTransform( float, float, Vector2 ) 
```
```c#
Matrix = Styles.BuildTransformMatrix( Vector2 ) 
```
```c#
Vector2 = Rect.Center { get; } 
```
```c#
Vector2 = GraphicsItem.Center { get; } 
```
```c#
Vector2 = VignetteSettings.Center { get; set; } 
```
```c#
void GraphicsView.CenterOn( Vector2 ) 
```
```c#
Vector2 = PlugIn.ConnectionPosition { get; } 
```
```c#
Vector2 = PlugOut.ConnectionPosition { get; } 
```
```c#
protected virtual void Panel.ConstrainScrolling( Vector2 ) 
```
```c#
virtual bool = GraphicsItem.Contains( Vector2 ) 
```
```c#
override bool = EditableCurve.Contains( Vector2 ) 
```
```c#
void MapStaticOverlay.CreateCenteredQuad( Vector2, Material ) 
```
```c#
void VoxelChunk.CreateModel( Vector2, Vector2, int, int, float, string, bool, byte[], int ) 
```
```c#
CommentUI = GraphView.CreateNewComment( string, CommentColor, Vector2, Vector2 ) 
```
```c#
NodeUI = GraphView.CreateNewNode( Type, Vector2 ) 
```
```c#
protected void GraphView.CreateNewNode( Type, Vector2, PlugOut, bool ) 
```
```c#
void GraphView.CreateNewReroute( Vector2 ) 
```
```c#
static Texture = Texture.CreateRenderTarget( string, ImageFormat, Vector2 ) 
```
```c#
static Texture = Texture.CreateRenderTarget( string, ImageFormat, Vector2, Texture ) 
```
```c#
static Matrix = Matrix.CreateSkew( Vector2 ) 
```
```c#
void GraphicsLine.CubicLineTo( Vector2, Vector2, Vector2 ) 
```
```c#
static Vector2 = Application.CursorDelta { get; } 
```
```c#
Vector2 = Inputs.CursorPosition { get; set; } 
```
```c#
static Vector2 = Application.CursorPosition { get; set; } 
```
```c#
static Vector2 = Mouse.Delta { get; } 
```
```c#
Vector2 = AnalogInput2D.Delta { get; } 
```
```c#
Vector2 = FloatRangeSlider.DeltaValue { get; set; } 
```
```c#
bool = GizmoControls.DragSquare( string, Vector2, Rotation, out Vector3, Action ) 
```
```c#
static void ToolRender.Draw2DCircle( Vector2, float, int, Color ) 
```
```c#
static void ToolRender.Draw2DCross( Vector2, Vector2, Color ) 
```
```c#
static void ToolRender.Draw2DRectangleFilled( Vector2, Vector2, Color ) 
```
```c#
static void ToolRender.Draw2DRectangleOutlined( Vector2, Vector2, Color ) 
```
```c#
static void ToolRender.Draw2DRectangleTextured( Vector2, Vector2, Texture, bool, bool ) 
```
```c#
static void Paint.DrawArc( Vector2, Vector2, float, float ) 
```
```c#
static void Paint.DrawArrow( Vector2, Vector2, float ) 
```
```c#
static void Paint.DrawCircle( Vector2, Vector2 ) 
```
```c#
static void Paint.DrawLine( IEnumerable<Vector2> ) 
```
```c#
static void Paint.DrawPie( Vector2, Vector2, float, float ) 
```
```c#
static void Paint.DrawPoints( IEnumerable<Vector2> ) 
```
```c#
static void Paint.DrawPolygon( IEnumerable<Vector2> ) 
```
```c#
static void ToolRender.DrawScreenText( string, Vector2, Color ) 
```
```c#
static void Paint.DrawSquare( Vector2, Vector2 ) 
```
```c#
static void ToolRender.DrawWorldSpaceText( string, Vector3, Vector2, Color, float ) 
```
```c#
Vector2 = Margin.EdgeSize { get; } 
```
```c#
Vector2 = SelectionBox.End { set; } 
```
```c#
Vector2 = SelectionEvent.EndPoint
```
```c#
Vector2 = BaseNode.ExpandSize { get; set; } 
```
```c#
Vector2 = ShatterGlass.FaceTexScale { get; set; } 
```
```c#
Vector2 = VoxelSurface.FaceTexScale { get; set; } 
```
```c#
Vector2 = ShatterGlass.FaceTexSize { get; set; } 
```
```c#
Vector2 = VoxelSurface.FaceTexSize { get; set; } 
```
```c#
override void Label.FinalLayout( Vector2 ) 
```
```c#
override void SvgPanel.FinalLayout( Vector2 ) 
```
```c#
virtual void Panel.FinalLayout( Vector2 ) 
```
```c#
protected virtual void Panel.FinalLayoutChildren( Vector2 ) 
```
```c#
protected override void VirtualScrollPanel.FinalLayoutChildren( Vector2 ) 
```
```c#
protected override void BaseVirtualScrollPanel<T>.FinalLayoutChildren( Vector2 ) 
```
```c#
Vector2 = GraphicsItem.FromItem( GraphicsItem, Vector2 ) 
```
```c#
Vector2 = GraphicsItem.FromItem( GraphicsItem, Vector2 ) 
```
```c#
Vector2 = GraphicsItem.FromParent( Vector2 ) 
```
```c#
Vector2 = GraphicsItem.FromParent( Vector2 ) 
```
```c#
Vector2 = GraphicsView.FromScene( Vector2 ) 
```
```c#
Vector2 = GraphicsView.FromScene( Vector2 ) 
```
```c#
Vector2 = GraphicsItem.FromScene( Vector2 ) 
```
```c#
Vector2 = GraphicsItem.FromScene( Vector2 ) 
```
```c#
Vector2 = Widget.FromScreen( Vector2 ) 
```
```c#
Vector2 = Widget.FromScreen( Vector2 ) 
```
```c#
static Vector2 = SandboxSystemExtensions.Gaussian2D( Random, Vector2?, Vector2? ) 
```
```c#
static Vector2 = SandboxSystemExtensions.Gaussian2D( Random, Vector2?, Vector2? ) 
```
```c#
static Vector2 = Input.GetAnalog( InputAnalog ) 
```
```c#
string = TextEdit.GetAnchorAt( Vector2 ) 
```
```c#
TextCursor = TextEdit.GetCursorAtPosition( Vector2 ) 
```
```c#
static Vector3 = Screen.GetDirection( Vector2 ) 
```
```c#
static Vector3 = Screen.GetDirection( Vector2, float ) 
```
```c#
static Vector3 = Screen.GetDirection( Vector2, float, Rotation ) 
```
```c#
static Vector3 = Screen.GetDirection( Vector2, float, Rotation, Vector2 ) 
```
```c#
Margin = Styles.GetInset( Vector2 ) 
```
```c#
GraphicsItem = GraphicsView.GetItemAt( Vector2 ) 
```
```c#
VirtualWidget = BaseItemWidget.GetItemAt( Vector2 ) 
```
```c#
int = Label.GetLetterAt( Vector2 ) 
```
```c#
int = Label.GetLetterAtScreenPosition( Vector2 ) 
```
```c#
static Ray = Screen.GetOrthoRay( Vector2 ) 
```
```c#
Margin = Styles.GetOutset( Vector2 ) 
```
```c#
abstract IPanel = IPanel.GetPanelAt( Vector2, bool, bool ) 
```
```c#
Vector2 = GlassShard.GetPanelVertexAverage( ) 
```
```c#
Ray = NativeRenderingWidget.GetRay( Vector2 ) 
```
```c#
virtual Vector2 = Panel.GetTransformPosition( Vector2 ) 
```
```c#
virtual Vector2 = Panel.GetTransformPosition( Vector2 ) 
```
```c#
Vector2 = WheelEvent.GlobalPosition { get; } 
```
```c#
virtual Vector2 = GraphicsItem.HandlePosition { get; set; } 
```
```c#
Vector2 = Result.HitTriangleUv { get; set; } 
```
```c#
virtual void TextureChangedDelegate.Invoke( ReadOnlySpan<byte>, Vector2 ) 
```
```c#
virtual void TextureChangedDelegate.Invoke( ReadOnlySpan<byte>, Vector2 ) 
```
```c#
bool = Panel.IsInside( Vector2 ) 
```
```c#
Vector2 = ListView.ItemSize { get; set; } 
```
```c#
Vector2 = ListView.ItemSpacing { get; set; } 
```
```c#
void GraphicsLine.LineTo( Vector2 ) 
```
```c#
Vector2 = DragEvent.LocalGrabPosition
```
```c#
Vector2 = DragEvent.LocalPosition
```
```c#
Vector2 = MousePanelEvent.LocalPosition
```
```c#
Vector2 = MouseEvent.LocalPosition { get; } 
```
```c#
Vector2 = ContextMenuEvent.LocalPosition { get; } 
```
```c#
Vector2 = GraphicsMouseEvent.LocalPosition { get; } 
```
```c#
Vector2 = GraphicsHoverEvent.LocalPosition { get; } 
```
```c#
Vector2 = DragEvent.LocalPosition { get; set; } 
```
```c#
Vector2 = ItemDragEvent.LocalPosition
```
```c#
Vector2 = Widget.MaximumSize { get; set; } 
```
```c#
Vector2 = FGDCurve.Maxs { get; } 
```
```c#
static Vector2 = Paint.MeasureText( string ) 
```
```c#
Vector2 = Widget.MinimumSize { get; set; } 
```
```c#
Vector2 = FGDCurve.Mins { get; } 
```
```c#
static Vector2 = Input.MouseDelta { get; set; } 
```
```c#
Vector2 = DragEvent.MouseDelta
```
```c#
Action<Vector2> = Widget.MouseMove
```
```c#
Vector2 = Panel.MousePosition { get; } 
```
```c#
Vector2 = MapView.MousePosition { get; } 
```
```c#
Vector2 = VROverlay.MouseScale { get; set; } 
```
```c#
void GraphicsLine.MoveTo( Vector2 ) 
```
```c#
void AutoComplete.OnAutoComplete( string, Vector2 ) 
```
```c#
static Rect = Rect.op_Addition( Rect, Vector2 ) 
```
```c#
static Vector3 = Vector3.op_Implicit( Vector2 ) 
```
```c#
static Vector2 = AnalogInput2D.op_Implicit( AnalogInput2D ) 
```
```c#
static Rect = Rect.op_Multiply( Rect, Vector2 ) 
```
```c#
static Margin = Margin.op_Multiply( Margin, Vector2 ) 
```
```c#
void AutoComplete.OpenAbove( Vector2 ) 
```
```c#
void Menu.OpenAt( Vector2, bool ) 
```
```c#
void PopupWidget.OpenAt( Vector2, bool, Vector2? ) 
```
```c#
void PopupWidget.OpenAtCursor( bool, Vector2? ) 
```
```c#
virtual void Handle.OpenContextMenu( Vector2 ) 
```
```c#
Vector2 = AutoComplete.OpenOffset { get; set; } 
```
```c#
Vector2 = Panel.PanelPositionToScreenPosition( Vector2 ) 
```
```c#
Vector2 = Panel.PanelPositionToScreenPosition( Vector2 ) 
```
```c#
Vector2 = ShatterGlass.PanelSize { get; } 
```
```c#
Pixmap.Pixmap( Vector2 ) 
```
```c#
IReadOnlyList<Vector2> = AddPolyPathCommand.Points { get; init; } 
```
```c#
Vector2 = Rect.Position { get; set; } 
```
```c#
Vector2 = Margin.Position { get; set; } 
```
```c#
static Vector2 = Mouse.Position { get; set; } 
```
```c#
Vector2 = WheelEvent.Position { get; } 
```
```c#
Vector2 = GraphicsItem.Position { get; set; } 
```
```c#
Vector2 = Widget.Position { get; set; } 
```
```c#
Vector2 = BaseNode.Position { get; set; } 
```
```c#
Vector2 = FloatControlWidget.Range { get; set; } 
```
```c#
Vector2 = ChartBackground.RangeX { get; set; } 
```
```c#
Vector2 = ChartBackground.RangeY { get; set; } 
```
```c#
static Vector2 = SandboxSystemExtensions.ReadVector2( BinaryReader ) 
```
```c#
Rect.Rect( Vector2, Vector2 ) 
```
```c#
Pixmap = Pixmap.Resize( Vector2 ) 
```
```c#
static void Paint.Rotate( float, Vector2 ) 
```
```c#
Vector2 = GraphicsView.Scale { get; set; } 
```
```c#
Vector2 = GraphicsMouseEvent.ScenePosition { get; } 
```
```c#
Vector2 = GraphicsHoverEvent.ScenePosition { get; } 
```
```c#
Vector2 = DragEvent.ScreenGrabPosition
```
```c#
Vector2 = DragEvent.ScreenPosition
```
```c#
Vector2 = MouseEvent.ScreenPosition { get; } 
```
```c#
Vector2 = ContextMenuEvent.ScreenPosition { get; } 
```
```c#
Vector2 = GraphicsMouseEvent.ScreenPosition { get; } 
```
```c#
Vector2 = GraphicsHoverEvent.ScreenPosition { get; } 
```
```c#
Vector2 = Widget.ScreenPosition { get; } 
```
```c#
Vector2 = AssetContextMenu.ScreenPosition
```
```c#
Vector2 = FolderContextMenu.ScreenPosition
```
```c#
Vector2 = CloudProjectRowContextMenu.ScreenPosition
```
```c#
Vector2 = ProjectRowContextMenu.ScreenPosition
```
```c#
Vector2 = Panel.ScreenPositionToPanelDelta( Vector2 ) 
```
```c#
Vector2 = Panel.ScreenPositionToPanelDelta( Vector2 ) 
```
```c#
Vector2 = Panel.ScreenPositionToPanelPosition( Vector2 ) 
```
```c#
Vector2 = Panel.ScreenPositionToPanelPosition( Vector2 ) 
```
```c#
virtual Vector2 = Slider2D.ScreenPositionToValue( Vector2 ) 
```
```c#
virtual Vector2 = Slider2D.ScreenPositionToValue( Vector2 ) 
```
```c#
virtual float = SliderControl.ScreenPosToValue( Vector2 ) 
```
```c#
void GizmoDraw.ScreenText( string, Vector2, string, float, TextFlag ) 
```
```c#
void DebugOverlay.ScreenText( string, Vector2, int, Color, float ) 
```
```c#
void DebugOverlay.ScreenText( string, Vector2, float ) 
```
```c#
Vector2 = Panel.ScrollOffset { get; set; } 
```
```c#
Vector2 = Panel.ScrollSize { get; } 
```
```c#
Vector2 = Panel.ScrollVelocity
```
```c#
SelectionBox.SelectionBox( Vector2, GraphicsView ) 
```
```c#
bool = Material.Set( string, Vector2 ) 
```
```c#
abstract void IPanel.SetAbsolutePosition( TextFlag, Vector2, float ) 
```
```c#
static void Paint.SetBrushLinear( Vector2, Vector2, Color, Color ) 
```
```c#
static void Paint.SetBrushRadial( Vector2, float, Color, Color ) 
```
```c#
static void Paint.SetBrushRadial( Vector2, float, float, Color, float, Color ) 
```
```c#
void ToolBar.SetIconSize( Vector2 ) 
```
```c#
bool = GlassShard.ShatterLocalSpace( Vector2 ) 
```
```c#
SimpleVertex.SimpleVertex( Vector3, Vector3, Vector3, Vector2 ) 
```
```c#
Vector2 = Rect.Size { get; set; } 
```
```c#
Vector2 = Margin.Size { get; set; } 
```
```c#
static Vector2 = Camera.Size { get; } 
```
```c#
Vector2 = Texture.Size { get; } 
```
```c#
Vector2 = SceneCamera.Size { get; set; } 
```
```c#
Vector2 = WebSurface.Size { get; set; } 
```
```c#
static Vector2 = Screen.Size { get; } 
```
```c#
virtual Vector2 = GraphicsItem.Size { get; set; } 
```
```c#
Vector2 = Pixmap.Size { get; } 
```
```c#
override Vector2 = GraphicsWidget.Size { get; set; } 
```
```c#
Vector2 = Widget.Size { get; set; } 
```
```c#
Vector2 = VoxelSurface.Size { get; } 
```
```c#
Vector2 = CommentNode.Size { get; set; } 
```
```c#
protected virtual Vector2 = Widget.SizeHint( ) 
```
```c#
protected override Vector2 = BBoxControlWidget.SizeHint( ) 
```
```c#
protected override Vector2 = BodyGroupsControlWidget.SizeHint( ) 
```
```c#
protected override Vector2 = BoolControlWidget.SizeHint( ) 
```
```c#
protected override Vector2 = ControlWidget.SizeHint( ) 
```
```c#
protected override Vector2 = CurveControlWidget.SizeHint( ) 
```
```c#
protected override Vector2 = GradientControlWidget.SizeHint( ) 
```
```c#
protected override Vector2 = StringControlWidget.SizeHint( ) 
```
```c#
protected override Vector2 = TransformControlWidget.SizeHint( ) 
```
```c#
protected override Vector2 = IconButton.SizeHint( ) 
```
```c#
protected override Vector2 = KeyBind.SizeHint( ) 
```
```c#
protected override Vector2 = ItemRow.SizeHint( ) 
```
```c#
protected override Vector2 = ToggleSwitch.SizeHint( ) 
```
```c#
void GizmoDraw.Sprite( Vector3, Vector2, Texture, bool ) 
```
```c#
Vector2 = SelectionEvent.StartPoint
```
```c#
void Instance.StompCursorPosition( Vector2 ) 
```
```c#
Vector2 = GlassShard.StressPosition { get; set; } 
```
```c#
void WebSurface.TellMouseMove( Vector2 ) 
```
```c#
Vector2 = SimpleVertex.texcoord
```
```c#
Vector2 = MeshVertex.TexCoord
```
```c#
void DebugOverlay.Texture( Texture, Vector2, float ) 
```
```c#
void DebugOverlay.Texture( Texture, Rect, Color, Vector2, Vector2, float ) 
```
```c#
Vector2 = Curve.TimeRange { get; set; } 
```
```c#
Vector2 = EditableCurve.TimeRange { get; } 
```
```c#
Vector2 = GraphicsItem.ToItem( GraphicsItem, Vector2 ) 
```
```c#
Vector2 = GraphicsItem.ToItem( GraphicsItem, Vector2 ) 
```
```c#
Vector2 = GraphicsItem.ToParent( Vector2 ) 
```
```c#
Vector2 = GraphicsItem.ToParent( Vector2 ) 
```
```c#
Vector2 = Rect.TopLeft { get; } 
```
```c#
Vector2 = Rect.TopRight { get; } 
```
```c#
Vector2 = GraphicsView.ToScene( Vector2 ) 
```
```c#
Vector2 = GraphicsView.ToScene( Vector2 ) 
```
```c#
Vector2 = GraphicsItem.ToScene( Vector2 ) 
```
```c#
Vector2 = GraphicsItem.ToScene( Vector2 ) 
```
```c#
Vector2 = SceneCamera.ToScreen( Vector3 ) 
```
```c#
static Vector2? = SandboxGameExtensions.ToScreen( Vector3, Vector2 ) 
```
```c#
static Vector2? = SandboxGameExtensions.ToScreen( Vector3, Vector2 ) 
```
```c#
Vector2 = Widget.ToScreen( Vector2 ) 
```
```c#
Vector2 = Widget.ToScreen( Vector2 ) 
```
```c#
Vector3 = GlassShard.TransformPosPanelToWorld( Vector2 ) 
```
```c#
Vector2 = GlassShard.TransformPosWorldToPanel( Vector3 ) 
```
```c#
void GraphicsView.Translate( Vector2 ) 
```
```c#
static void Paint.Translate( Vector2 ) 
```
```c#
static Vector2 = Application.UnscaledCursorPosition { get; set; } 
```
```c#
bool = Pixmap.UpdateFromPixels( ReadOnlySpan<byte>, Vector2, ImageFormat ) 
```
```c#
void CurveEditor.UpdateTimeRange( Vector2 ) 
```
```c#
void CurveEditor.UpdateValueRange( Vector2 ) 
```
```c#
Vector2 = VertexDetail.Uv0 { get; set; } 
```
```c#
Vector2 = VertexDetail.Uv1 { get; set; } 
```
```c#
Vector2 = AnalogInput2D.Value { get; } 
```
```c#
Vector2 = Slider2D.Value { get; set; } 
```
```c#
Vector2 = FloatRangeSlider.Value { get; set; } 
```
```c#
Vector2 = FloatRangeSliderProperty.Value { get; set; } 
```
```c#
Vector2 = Vector2Property.Value { get; set; } 
```
```c#
Vector2 = Curve.ValueRange { get; set; } 
```
```c#
Vector2 = EditableCurve.ValueRange { get; } 
```
```c#
Vector2 = AsAccessor.Vector2 { get; set; } 
```
```c#
Vector3.Vector3( Vector2, float ) 
```
```c#
static Vector2 = SandboxSystemExtensions.VectorInCircle( Random, float ) 
```
```c#
static Vector2 = SandboxSystemExtensions.VectorInSquare( Random, float ) 
```
```c#
static Vector2 = Mouse.Velocity { get; } 
```
```c#
Vector2 = GraphicsItem.ViewPosition { get; } 
```
```c#
Vector2 = RippleConstants.ViewPosition
```
```c#
Vector2 = RippleConstants.ViewPositionLast
```
```c#
Vector2 = MouseEvent.WindowPosition { get; } 
```
```c#
Texture2DBuilder = Texture2DBuilder.WithSize( Vector2 ) 
```
```c#
TextureBuilder = TextureBuilder.WithSize( Vector2 ) 
```
```c#
TextureCubeBuilder = TextureCubeBuilder.WithSize( Vector2 ) 
```
```c#
static void SandboxSystemExtensions.Write( BinaryWriter, Vector2 ) 
```
```c#
void GraphicsView.Zoom( float, Vector2 ) 
```
