# Length

## 
```c#
Implements IEquatable<Length>
```

## Summary

A variable unit based length. ie, could be a percentage or a pixel length. This is commonly used to express the size of things in UI space, usually coming from style sheets.
## Fields

```c#
LengthUnit Unit
```
How to determine the final length. Commonly used with Pixel or Percentage.
```c#
float Value
```
The meaning of the value is dependent onLength.Unit.
## Properties

```c#
static Length Auto { get; } 
```
Quickly create a Length with Unit set to LengthUnit.Auto
```c#
static Length Contain { get; } 
```
Quickly create a Length with Unit set to LengthUnit.Contain
```c#
static Length Cover { get; } 
```
Quickly create a Length with Unit set to LengthUnit.Cover
```c#
static Length Undefined { get; } 
```
No Summary
## Methods

```c#
static Length? Fraction( float fraction) 
```
Create a length in percents
```c#
static Length? Parse( string value) 
```
Parse a length. This is used by the stylesheet parsing system.
```c#
static Length? Percent( float percent) 
```
Create a length in percents
```c#
static Length? Pixels( float pixels) 
```
Create a length in pixels
```c#
static Length? ViewHeight( float percentage) 
```
Create a length based on the view height
```c#
static Length? ViewMax( float percentage) 
```
Create a length based on the longest edge of the screen size
```c#
static Length? ViewMin( float percentage) 
```
Create a length based on the shortest edge of the screen size
```c#
static Length? ViewWidth( float percentage) 
```
Create a length based on the view width
```c#
float GetPixels( float dimension) 
```
Convert to a pixel value. Use the dimension to work out percentage values.
```c#
float GetPixels( float dimension, float contentSize) 
```
Get the pixel size but also evaluate content size to support use Start, End, Center
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( Length other) 
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
bool ==( Length lhs, Length rhs) 
```
No Summary
```c#
bool ==( Length? lhs, Length? rhs) 
```
No Summary
```c#
bool !=( Length lhs, Length rhs) 
```
No Summary
```c#
bool !=( Length? lhs, Length? rhs) 
```
No Summary
```c#
implicit Length =( float value) 
```
No Summary
## Referencing Members

```c#
bool = PanelTransform.AddPerspective( Length ) 
```
```c#
bool = PanelTransform.AddTranslate( Length?, Length?, Length? ) 
```
```c#
bool = PanelTransform.AddTranslateX( Length? ) 
```
```c#
bool = PanelTransform.AddTranslateY( Length? ) 
```
```c#
bool = PanelTransform.AddTranslateZ( Length? ) 
```
```c#
Length? = BaseStyles.BackdropFilterBlur { get; set; } 
```
```c#
Length? = BaseStyles.BackdropFilterBrightness { get; set; } 
```
```c#
Length? = BaseStyles.BackdropFilterContrast { get; set; } 
```
```c#
Length? = BaseStyles.BackdropFilterHueRotate { get; set; } 
```
```c#
Length? = BaseStyles.BackdropFilterInvert { get; set; } 
```
```c#
Length? = BaseStyles.BackdropFilterSaturate { get; set; } 
```
```c#
Length? = BaseStyles.BackdropFilterSepia { get; set; } 
```
```c#
Length? = BaseStyles.BackgroundAngle { get; set; } 
```
```c#
Length? = BaseStyles.BackgroundPositionX { get; set; } 
```
```c#
Length? = BaseStyles.BackgroundPositionY { get; set; } 
```
```c#
Length? = BaseStyles.BackgroundSizeX { get; set; } 
```
```c#
Length? = BaseStyles.BackgroundSizeY { get; set; } 
```
```c#
Length? = BaseStyles.BorderBottomLeftRadius { get; set; } 
```
```c#
Length? = BaseStyles.BorderBottomRightRadius { get; set; } 
```
```c#
Length? = BaseStyles.BorderBottomWidth { get; set; } 
```
```c#
Length? = BaseStyles.BorderImageWidthBottom { get; set; } 
```
```c#
Length? = BaseStyles.BorderImageWidthLeft { get; set; } 
```
```c#
Length? = BaseStyles.BorderImageWidthRight { get; set; } 
```
```c#
Length? = BaseStyles.BorderImageWidthTop { get; set; } 
```
```c#
Length? = BaseStyles.BorderLeftWidth { get; set; } 
```
```c#
Length? = BaseStyles.BorderRightWidth { get; set; } 
```
```c#
Length? = BaseStyles.BorderTopLeftRadius { get; set; } 
```
```c#
Length? = BaseStyles.BorderTopRightRadius { get; set; } 
```
```c#
Length? = BaseStyles.BorderTopWidth { get; set; } 
```
```c#
Length? = Styles.BorderWidth { set; } 
```
```c#
Length? = BaseStyles.Bottom { get; set; } 
```
```c#
Length? = BaseStyles.ColumnGap { get; set; } 
```
```c#
Length? = BaseStyles.FilterBlur { get; set; } 
```
```c#
Length? = BaseStyles.FilterBorderWidth { get; set; } 
```
```c#
Length? = BaseStyles.FilterBrightness { get; set; } 
```
```c#
Length? = BaseStyles.FilterContrast { get; set; } 
```
```c#
Length? = BaseStyles.FilterHueRotate { get; set; } 
```
```c#
Length? = BaseStyles.FilterInvert { get; set; } 
```
```c#
Length? = BaseStyles.FilterSaturate { get; set; } 
```
```c#
Length? = BaseStyles.FilterSepia { get; set; } 
```
```c#
Length? = BaseStyles.FlexBasis { get; set; } 
```
```c#
Length? = BaseStyles.FontSize { get; set; } 
```
```c#
Length? = BaseStyles.Height { get; set; } 
```
```c#
Length = GridLayout.ItemHeight { get; set; } 
```
```c#
Length = GridLayout.ItemWidth { get; set; } 
```
```c#
Length? = BaseStyles.Left { get; set; } 
```
```c#
protected void BaseStyles.Lerp( string, ref Length?, Length?, Length?, Length?, float ) 
```
```c#
Length? = BaseStyles.LetterSpacing { get; set; } 
```
```c#
Length? = BaseStyles.LineHeight { get; set; } 
```
```c#
Length? = Styles.Margin { set; } 
```
```c#
Length? = BaseStyles.MarginBottom { get; set; } 
```
```c#
Length? = BaseStyles.MarginLeft { get; set; } 
```
```c#
Length? = BaseStyles.MarginRight { get; set; } 
```
```c#
Length? = BaseStyles.MarginTop { get; set; } 
```
```c#
Length? = BaseStyles.MaskAngle { get; set; } 
```
```c#
Length? = BaseStyles.MaskPositionX { get; set; } 
```
```c#
Length? = BaseStyles.MaskPositionY { get; set; } 
```
```c#
Length? = BaseStyles.MaskSizeX { get; set; } 
```
```c#
Length? = BaseStyles.MaskSizeY { get; set; } 
```
```c#
Length? = BaseStyles.MaxHeight { get; set; } 
```
```c#
Length? = BaseStyles.MaxWidth { get; set; } 
```
```c#
Length? = BaseStyles.MinHeight { get; set; } 
```
```c#
Length? = BaseStyles.MinWidth { get; set; } 
```
```c#
Length? = Styles.Padding { set; } 
```
```c#
Length? = BaseStyles.PaddingBottom { get; set; } 
```
```c#
Length? = BaseStyles.PaddingLeft { get; set; } 
```
```c#
Length? = BaseStyles.PaddingRight { get; set; } 
```
```c#
Length? = BaseStyles.PaddingTop { get; set; } 
```
```c#
Length? = BaseStyles.PerspectiveOriginX { get; set; } 
```
```c#
Length? = BaseStyles.PerspectiveOriginY { get; set; } 
```
```c#
Length? = BaseStyles.Right { get; set; } 
```
```c#
Length? = BaseStyles.RowGap { get; set; } 
```
```c#
Length? = BaseStyles.TextBackgroundAngle { get; set; } 
```
```c#
Length? = BaseStyles.TextDecorationThickness { get; set; } 
```
```c#
Length? = BaseStyles.TextLineThroughOffset { get; set; } 
```
```c#
Length? = BaseStyles.TextOverlineOffset { get; set; } 
```
```c#
Length? = BaseStyles.TextStrokeWidth { get; set; } 
```
```c#
Length? = BaseStyles.TextUnderlineOffset { get; set; } 
```
```c#
Length? = BaseStyles.Top { get; set; } 
```
```c#
Length? = BaseStyles.TransformOriginX { get; set; } 
```
```c#
Length? = BaseStyles.TransformOriginY { get; set; } 
```
```c#
Length? = BaseStyles.Width { get; set; } 
```
```c#
Length? = BaseStyles.WordSpacing { get; set; } 
```
```c#
Length = Entry.X
```
```c#
Length = Entry.Y
```
```c#
Length = Entry.Z
```
