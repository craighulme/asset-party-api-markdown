# Color

## Derives from ValueType
Implements IEquatable< Color>

## Summary

Initialize a color with each component set to given values, in range [0,1]
## Constructors

```c#
Color( float r, float g, float b, float a = 1) 
```
Initialize a color with each component set to given values, in range [0,1]
```c#
Color( float all) 
```
Initialize a color with each component set to given value, even alpha.
```c#
Color( uint raw) 
```
Initialize from an integer of the form 0xAABBGGRR.
```c#
Color( int raw) 
```
Initialize from an integer of the form 0xAABBGGRR.
## Fields

```c#
static readonly Color Black
```
Fully opaque black color.
```c#
static readonly Color Blue
```
Fully opaque pure blue color.
```c#
static readonly Color Cyan
```
Fully opaque cyan color.
```c#
static readonly Color Gray
```
Fully opaque gray color, right between white and black.
```c#
static readonly Color Green
```
Fully opaque pure green color.
```c#
static readonly Color Magenta
```
Fully opaque magenta color.
```c#
static readonly Color Orange
```
Fully opaque orange color.
```c#
static readonly Color Red
```
Fully opaque pure red color.
```c#
static readonly Color Transparent
```
Fully transparent color.
```c#
static readonly Color White
```
Fully opaque white color.
```c#
static readonly Color Yellow
```
Fully opaque yellow color.
```c#
float a
```
The alpha/transparency color component, in range of 0 (fully transparent) to 1 (fully opaque), whichcan be exceeded.
```c#
float b
```
The blue color component, in range of 0-1, whichcan be exceeded.
```c#
float g
```
The green color component, in range of 0-1, whichcan be exceeded.
```c#
float r
```
The red color component, in range of 0-1, whichcan be exceeded.
## Properties

```c#
static Color Random { get; } 
```
Returns a random color out of 8 preset colors.
```c#
string Hex { get; } 
```
String representation of the form "#RRGGBB[AA]".
```c#
bool IsHdr { get; } 
```
Returns true if any component exceeds 1
```c#
bool IsRepresentableInHex { get; } 
```
Returns true if this color can be represented in hexadecimal format (#RRGGBB[AA]).
This may not be the case if the color components are outside of [0,1] range.
```c#
bool IsSdr { get; } 
```
Returns true if all components are between 0 and 1
```c#
float Luminance { get; } 
```
Returns the luminance of the color, basically it's grayscale value or "black and white version".
```c#
uint RawInt { get; } 
```
Integer representation of the form 0xAABBGGRR as used by native code.
```c#
string Rgb { get; } 
```
String representation in the form ofrgb( r, g, b )
css function notation.
```c#
string Rgba { get; } 
```
String representation in the form ofrgba( r, g, b, a )
css function notation.
```c#
uint RgbaInt { get; } 
```
Integer representation of the form 0xRRGGBBAA.
```c#
uint RgbInt { get; } 
```
Integer representation of the form 0xRRGGBB.
## Methods

```c#
static Color Average( Color[] values) 
```
Returns a color whose components are averaged of all given colors.
```c#
static Color FromBytes( int r, int g, int b, int a = 255) 
```
Creates a color from 0-255 range inputs, converting them to 0-1 range.
```c#
static Color FromRgb( uint rgb) 
```
Converts an integer of the form 0xRRGGBB into the color #RRGGBB with 100% alpha.
```c#
static Color FromRgba( uint rgba) 
```
Converts an integer of the form 0xRRGGBBAA into the color #RRGGBBAA.
```c#
static Color Lerp( Color a, Color b, float frac, bool clamped = true) 
```
Performs linear interpolation between two colors.
```c#
static Color Max( Color a, Color b) 
```
Returns a new color with each component being the maximum of the 2 given colors.
```c#
static Color Min( Color a, Color b) 
```
Returns a new color with each component being the minimum of the 2 given colors.
```c#
static Color? Parse( string value) 
```
Parse the color from a string. Many common formats are supported.
```c#
static Color Read( BinaryReader reader) 
```
Read a color from binary reader.
```c#
static bool TryParse( string value, out Color color) 
```
Try to parse the color. Returns true on success
```c#
Color AdjustHue( float amount) 
```
Increases or decreases this color's hue
```c#
int ComponentCountChangedBetweenColors( Color b) 
```
Returns how many color components would be changed between this color and another color
```c#
Color Darken( float fraction) 
```
Darkens the color by given amount.
```c#
Color Desaturate( float fraction) 
```
Desaturates the color by given amount.
```c#
Color Invert( ) 
```
Returns inverted color. Alpha is unchanged.
```c#
Color Lighten( float fraction) 
```
Lightens the color by given amount.
```c#
Color Saturate( float fraction) 
```
Saturates the color by given amount.
```c#
Color32 ToColor32( bool srgb = false) 
```
Convert to a Color32 (a 32 bit color value)
```c#
ColorHsv ToHsv( ) 
```
Converts this color to a HSV format.
```c#
string ToString( bool hex, bool rgba) 
```
Converts the color to a string with given parameters.
```c#
Color WithAlpha( float alpha) 
```
Returns this color with its alpha value changed
```c#
Color WithAlphaMultiplied( float alpha) 
```
Similar toColor.WithAlphabut multiplies the alpha instead of replacing.
```c#
Color WithBlue( float blue) 
```
Returns this color with its blue value changed
```c#
Color WithGreen( float green) 
```
Returns this color with its green value changed
```c#
Color WithRed( float red) 
```
Returns this color with its red value changed
```c#
void Write( BinaryWriter writer) 
```
Write this color to a binary writer.
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( Color o) 
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
float this[ int index, ] 
```
Get color components by numerical index.
```c#
Color +( Color c1, Color c2) 
```
No Summary
```c#
bool ==( Color left, Color right) 
```
No Summary
```c#
bool !=( Color left, Color right) 
```
No Summary
```c#
Color *( Color c1, float f) 
```
Multiply each component of this color by given value.
```c#
Color -( Color c1, Color c2) 
```
No Summary
```c#
implicit Color =( Vector4 value) 
```
No Summary
```c#
implicit Color =( Vector3 value) 
```
No Summary
```c#
implicit Color =( Color32 color) 
```
No Summary
```c#
implicit Color =( string value) 
```
No Summary
## Referencing Members

```c#
static Color = Colors.Active { get; } 
```
```c#
Color = EnvironmentLightEntity.AmbientColor { get; set; } 
```
```c#
Color = SceneCamera.AmbientLightColor { get; set; } 
```
```c#
Color = SceneWorld.AmbientLightColor
```
```c#
Color? = IconAttribute.BackgroundColor { get; } 
```
```c#
Color = SceneCamera.BackgroundColor { get; set; } 
```
```c#
Color? = BaseStyles.BackgroundColor { get; set; } 
```
```c#
Color = WarningBox.BackgroundColor { get; set; } 
```
```c#
Color = IconWidget.BackgroundColor { get; set; } 
```
```c#
Color? = BaseStyles.BackgroundTint { get; set; } 
```
```c#
static Color = Theme.Black
```
```c#
static Color = Colors.Blue { get; } 
```
```c#
static Color = Theme.Blue
```
```c#
Color = BloomAccessor.BlurTint0 { get; set; } 
```
```c#
Color = BloomAccessor.BlurTint1 { get; set; } 
```
```c#
Color = BloomAccessor.BlurTint2 { get; set; } 
```
```c#
Color = BloomAccessor.BlurTint3 { get; set; } 
```
```c#
Color = BloomAccessor.BlurTint4 { get; set; } 
```
```c#
Color? = BaseStyles.BorderBottomColor { get; set; } 
```
```c#
Color? = Styles.BorderColor { set; } 
```
```c#
Color = NoticeWidget.BorderColor
```
```c#
Color? = BaseStyles.BorderImageTint { get; set; } 
```
```c#
Color? = BaseStyles.BorderLeftColor { get; set; } 
```
```c#
Color? = BaseStyles.BorderRightColor { get; set; } 
```
```c#
Color? = BaseStyles.BorderTopColor { get; set; } 
```
```c#
void DebugOverlay.Box( Vector3, Vector3, Color, float, bool ) 
```
```c#
void DebugOverlay.Box( Vector3, Vector3, Vector3, Color, float, bool ) 
```
```c#
void DebugOverlay.Box( Vector3, Rotation, Vector3, Vector3, Color, float, bool ) 
```
```c#
void DebugOverlay.Box( Entity, Color, float ) 
```
```c#
void DebugOverlay.Box( PhysicsBody, Color, float ) 
```
```c#
void DebugOverlay.Box( BBox, Color, float ) 
```
```c#
static void Breakables.Break( Model, Vector3, Rotation, float, Color, Result, PhysicsBody ) 
```
```c#
static Color = Theme.ButtonDefault
```
```c#
Color = TextEntry.CaretColor { get; set; } 
```
```c#
void DebugOverlay.Circle( Vector3, Rotation, float, Color, float, bool ) 
```
```c#
static void Graphics.Clear( Color, bool, bool, bool ) 
```
```c#
static void Graphics.Clear( Color, bool, bool ) 
```
```c#
void Pixmap.Clear( Color ) 
```
```c#
Color = ScenePortal.ClearColor { set; } 
```
```c#
Color = SceneWorld.ClearColor
```
```c#
Color = GradientColorOffset.color
```
```c#
static Color = SandboxSystemExtensions.Color( Random ) 
```
```c#
Color = Shadow.Color
```
```c#
Color = GradientFogController.Color { get; set; } 
```
```c#
Color = GizmoDraw.Color { get; set; } 
```
```c#
Color = Vertex.Color
```
```c#
Color = EnvironmentLightEntity.Color { get; set; } 
```
```c#
Color = OrthoLightEntity.Color { get; set; } 
```
```c#
Color = PointLightEntity.Color { get; set; } 
```
```c#
Color = SpotLightEntity.Color { get; set; } 
```
```c#
static Color = Game.Color { get; } 
```
```c#
Color = VROverlay.Color { get; set; } 
```
```c#
Color = Label.Color { get; set; } 
```
```c#
Color = WorldTextEntity.Color { get; set; } 
```
```c#
Color = Glow.Color { get; set; } 
```
```c#
Color = VignetteSettings.Color { get; set; } 
```
```c#
Color = HandleConfig.Color { get; set; } 
```
```c#
Color = TagDetail.Color { get; set; } 
```
```c#
Color = Option.Color
```
```c#
ColorFrame.ColorFrame( float, Color ) 
```
```c#
ColorPicker.ColorPicker( Widget, Color ) 
```
```c#
Color = SceneObject.ColorTint { get; set; } 
```
```c#
protected Color = GradientEditorWidget.ColorValue { get; set; } 
```
```c#
ColouredLabel.ColouredLabel( Color, string ) 
```
```c#
static Color = Theme.ControlBackground
```
```c#
static Color = ControlWidget.ControlColor
```
```c#
static Color = ControlWidget.ControlHighlightPrimary
```
```c#
static Color = ControlWidget.ControlHighlightSecondary
```
```c#
static Color = Theme.ControlText
```
```c#
Color = EditableCurve.CurveColor { get; set; } 
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
static void ToolRender.DrawBox( Vector3, Vector3, Color ) 
```
```c#
static Rect = Graphics.DrawIcon( Rect, string, Color, float, TextFlag ) 
```
```c#
static void ToolRender.DrawLine( Vector3, Vector3, Color, Color ) 
```
```c#
static void ToolRender.DrawLine( Vector3, Vector3, Color ) 
```
```c#
static void ToolRender.DrawScreenText( string, Vector2, Color ) 
```
```c#
static Rect = Graphics.DrawText( in Rect, string, Color, string, float, float, TextFlag ) 
```
```c#
static Rect = Graphics.DrawText( in Vector2, string, Color, string, float, float ) 
```
```c#
static Rect = Paint.DrawTextBox( Rect, string, Color, Margin, float, TextFlag ) 
```
```c#
static void ToolRender.DrawWorldSpaceText( string, Vector3, Vector2, Color, float ) 
```
```c#
Color = EditorModelAttribute.DynamicColor { get; set; } 
```
```c#
Color = Gradient.Evaluate( float ) 
```
```c#
Color? = SvgPath.FillColor { get; } 
```
```c#
Color? = BaseStyles.FilterBorderColor { get; set; } 
```
```c#
Color? = BaseStyles.FilterTint { get; set; } 
```
```c#
Color = GradientFogEntity.FogColor { get; set; } 
```
```c#
Color? = BaseStyles.FontColor { get; set; } 
```
```c#
Color? = IconAttribute.ForegroundColor { get; } 
```
```c#
Color = IconWidget.ForegroundColor { get; set; } 
```
```c#
static Color = Colors.Forward { get; } 
```
```c#
Color = ColorGradient.GetColor( float ) 
```
```c#
Color = CommentNode.GetColor( ) 
```
```c#
Color = VirtualWidget.GetForegroundColor( ) 
```
```c#
static Color = Colors.Green { get; } 
```
```c#
static Color = Theme.Green
```
```c#
static Color = Theme.Grey
```
```c#
Color = Curve2DProperty.HighlightColor
```
```c#
Color = CurveControlWidget.HighlightColor
```
```c#
Color = FloatControlWidget.HighlightColor { get; set; } 
```
```c#
Color = FloatingPointProperty<T>.HighlightColor
```
```c#
Color = FloatSlider.HighlightColor { get; set; } 
```
```c#
Color = FloatSliderProperty.HighlightColor { get; set; } 
```
```c#
Color = IntProperty.HighlightColor
```
```c#
Color = FloatRangeSlider.HighlightColor { get; set; } 
```
```c#
Color = FloatRangeSliderProperty.HighlightColor { get; set; } 
```
```c#
static Color = Colors.Hovered { get; } 
```
```c#
Color = Header.IconColor { get; set; } 
```
```c#
Color = Section.IconColor { get; set; } 
```
```c#
Color = Glow.InsideColor { get; set; } 
```
```c#
Color = Glow.InsideObscuredColor { get; set; } 
```
```c#
Color = AxisConfig.LabelColor { get; set; } 
```
```c#
static Color = Colors.Left { get; } 
```
```c#
protected void BaseStyles.Lerp( string, ref Color?, Color?, Color?, Color?, float ) 
```
```c#
Color = SceneLight.LightColor { get; set; } 
```
```c#
void DebugOverlay.Line( Vector3, Vector3, Color, float, bool ) 
```
```c#
Color = AxisConfig.LineColor { get; set; } 
```
```c#
Color = Glow.ObscuredColor { get; set; } 
```
```c#
static Color32 = Color32.op_Implicit( Color ) 
```
```c#
static ColorHsv = ColorHsv.op_Implicit( Color ) 
```
```c#
static Color = ColorHsv.op_Implicit( ColorHsv ) 
```
```c#
static Vector3 = Vector3.op_Implicit( Color ) 
```
```c#
static Gradient = Gradient.op_Implicit( Color ) 
```
```c#
static void ColorPicker.OpenColorPopup( Color, Action<Color> ) 
```
```c#
List<Color> = ColorPalette.Options { get; set; } 
```
```c#
void VirtualWidget.PaintBackground( Color, float ) 
```
```c#
static void ColorPalette.PaintSwatch( Color, Rect, bool, float, bool ) 
```
```c#
Color = PrecipitationEntity.ParticleTint { get; set; } 
```
```c#
static Color = Theme.Pink
```
```c#
static Color = Colors.Pitch { get; } 
```
```c#
static SceneObject = Decal.Place( SceneWorld, Material, Vector3, Rotation, Vector3, Color ) 
```
```c#
static void Decal.Place( To, DecalDefinition, Entity, int, Vector3, Rotation, Color ) 
```
```c#
static void Decal.Place( DecalDefinition, Entity, int, Vector3, Rotation, Color ) 
```
```c#
static void Decal.Place( DecalDefinition, TraceResult, Color ) 
```
```c#
static void Decal.Place( DecalDefinition, Vector3, Rotation, Color ) 
```
```c#
static Color = Theme.Primary
```
```c#
Color = NodeUI.PrimaryColor
```
```c#
static Color = SandboxSystemExtensions.ReadColor( BinaryReader ) 
```
```c#
static Color = Colors.Red { get; } 
```
```c#
static Color = Theme.Red
```
```c#
static void Graphics.Render( SceneObject, Transform?, Color?, Material ) 
```
```c#
Color = ModelEntity.RenderColor { get; set; } 
```
```c#
static Color = Colors.Roll { get; } 
```
```c#
bool = GizmoControls.RotateSingle( string, Rotation, Color, out Rotation, float ) 
```
```c#
SceneLight.SceneLight( SceneWorld, Vector3, float, Color ) 
```
```c#
SceneSpotLight.SceneSpotLight( SceneWorld, Vector3, Color ) 
```
```c#
SceneSunLight.SceneSunLight( SceneWorld, Rotation, Color ) 
```
```c#
static IDisposable = Superluminal.Scope( string, Color, string ) 
```
```c#
void DebugOverlay.ScreenText( string, Vector2, int, Color, float ) 
```
```c#
static Color = Colors.Selected { get; } 
```
```c#
static Color = Theme.Selection
```
```c#
Color = EditableCurve.SelectionColor { get; set; } 
```
```c#
Color = NodeUI.SelectionOutline
```
```c#
bool = Material.Set( string, Color ) 
```
```c#
static void Paint.SetBrush( Color ) 
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
void GradientFogEntity.SetFogColor( Color ) 
```
```c#
void OrthoLightEntity.SetLightColor( Color ) 
```
```c#
void PointLightEntity.SetLightColor( Color ) 
```
```c#
void SpotLightEntity.SetLightColor( Color ) 
```
```c#
static void Paint.SetPen( Color, float, PenStyle ) 
```
```c#
bool = DebugOverlay.Skeleton( Entity, Color, float, bool ) 
```
```c#
Color = SceneSunLight.SkyColor { get; set; } 
```
```c#
Color = EnvironmentLightEntity.SkyColor { get; set; } 
```
```c#
Color = SceneSkyBox.SkyTint { get; set; } 
```
```c#
void DebugOverlay.Sphere( Vector3, float, Color, float, bool ) 
```
```c#
void DebugOverlay.Sphere( Sphere, Color, float ) 
```
```c#
Color = EditorModelAttribute.StaticColor { get; set; } 
```
```c#
Color? = SvgPath.StrokeColor { get; } 
```
```c#
void DebugOverlay.Text( string, Vector3, int, Color, float, float ) 
```
```c#
void DebugOverlay.Text( string, Vector3, Color, float, float ) 
```
```c#
Color? = BaseStyles.TextDecorationColor { get; set; } 
```
```c#
Color? = BaseStyles.TextStrokeColor { get; set; } 
```
```c#
void DebugOverlay.Texture( Texture, Rect, Color, Vector2, Vector2, float ) 
```
```c#
Color = SceneCubemap.TintColor { get; set; } 
```
```c#
Color = Sky.TintColor { get; set; } 
```
```c#
Color = ParticleSystemEntity.TintControlPointColor { get; set; } 
```
```c#
Color = Color32.ToColor( ) 
```
```c#
Color = Color32.ToColor( bool ) 
```
```c#
Color = ColorHsv.ToColor( ) 
```
```c#
static Color = Colors.Up { get; } 
```
```c#
Color = ColorFrame.Value { get; set; } 
```
```c#
Color = ColorProperty.Value { get; set; } 
```
```c#
Color = ColorPalette.Value { get; set; } 
```
```c#
Color = ColorPicker.Value { get; set; } 
```
```c#
Color = ColorEditor.Value { get; set; } 
```
```c#
Action<Color> = ColorPicker.ValueChanged { get; set; } 
```
```c#
Color = ColorPicker.ValueWithoutRange { get; } 
```
```c#
static Color = Theme.White
```
```c#
static Color = Theme.WidgetBackground
```
```c#
static Color = Theme.WindowBackground
```
```c#
static void SandboxSystemExtensions.Write( BinaryWriter, Color ) 
```
```c#
static Color = Colors.Yaw { get; } 
```
```c#
static Color = Theme.Yellow
```
