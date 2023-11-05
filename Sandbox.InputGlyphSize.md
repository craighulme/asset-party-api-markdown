# InputGlyphSize

## ```c#
Derives from Enum
```

## Summary

Large 256x256 ( Keyboard glyphs can be wider for long key names )
## Fields

```c#
static InputGlyphSize Large = 2
```
Large 256x256 ( Keyboard glyphs can be wider for long key names )
```c#
static InputGlyphSize Medium = 1
```
Medium 128x128 ( Keyboard glyphs can be wider for long key names )
```c#
static InputGlyphSize Small = 0
```
Small 32x32 ( Keyboard glyphs can be wider for long key names )
## Extensions

```c#
int ToPixels( ) 
```
Translates this enum to pixel size.
## Referencing Members

```c#
static Texture = Input.GetGlyph( string, InputGlyphSize, GlyphStyle ) 
```
```c#
static Texture = Input.GetGlyph( InputAnalog, InputGlyphSize ) 
```
```c#
static Texture = Input.GetGlyph( InputButton, InputGlyphSize, GlyphStyle ) 
```
```c#
static int = SandboxGameExtensions.ToPixels( InputGlyphSize ) 
```
