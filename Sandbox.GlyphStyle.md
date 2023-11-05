# GlyphStyle

## Derives from ValueType

## Summary

White detail/borders on a black background
## Fields

```c#
static readonly GlyphStyle Dark
```
White detail/borders on a black background
```c#
static readonly GlyphStyle Knockout
```
Face buttons will have colored labels/outlines on a knocked out background
Rest of inputs will have white detail/borders on a knocked out background
```c#
static readonly GlyphStyle Light
```
Black detail/borders on a white background
## Methods

```c#
GlyphStyle WithNeutralColorABXY( ) 
```
ABXY Buttons will match the base style color instead of their normal associated color
```c#
GlyphStyle WithSolidABXY( ) 
```
ABXY Buttons will have a solid fill
## Referencing Members

```c#
static Texture = Input.GetGlyph( string, InputGlyphSize, GlyphStyle ) 
```
```c#
static Texture = Input.GetGlyph( InputButton, InputGlyphSize, GlyphStyle ) 
```
