# ColorHsv

## Derives from ValueType
Implements IEquatable< ColorHsv>

## Summary

A color inHue-Saturation-Value/Brightnessformat.
## Constructors

```c#
ColorHsv( float h, float s, float v, float a = 1) 
```
Initializes a new HSV/HSB color. Hue is in the range of [0-360] and all other values are in range [0,1]
## Properties

```c#
float Alpha { get; set; } 
```
Transparency of this color in range 0 (fully transparent) to 1 (fully opaque).
```c#
float Hue { get; set; } 
```
Hue component of this color in range 0 to 360.
```c#
float Saturation { get; set; } 
```
Saturation of this color in range 0 (white) to 1 (full color).
```c#
float Value { get; set; } 
```
Brightness of this color in range 0 (black) to 1 (full color).
## Methods

```c#
Color ToColor( ) 
```
Convert this object toColor.
```c#
ColorHsv WithAlpha( float alpha) 
```
Returns a copy of this color with given alpha value.
```c#
ColorHsv WithHue( float hue) 
```
Returns a copy of this color with given Hue value.
```c#
ColorHsv WithSaturation( float saturation) 
```
Returns a copy of this color with given Saturation value.
```c#
ColorHsv WithValue( float value) 
```
Returns a copy of this color with given Brightness value.
```c#
override bool Equals( object obj) 
```
OverridesValueType.Equals
```c#
override bool Equals( ColorHsv o) 
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
bool ==( ColorHsv left, ColorHsv right) 
```
No Summary
```c#
bool !=( ColorHsv left, ColorHsv right) 
```
No Summary
```c#
implicit ColorHsv =( Color rgb) 
```
No Summary
```c#
implicit Color =( ColorHsv hsv) 
```
No Summary
## Referencing Members

```c#
ColorHsv = Color.ToHsv( ) 
```
