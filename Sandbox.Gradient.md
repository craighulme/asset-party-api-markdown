# Gradient

## Derives from ValueType

## Summary

Describes a gradient between multiple colors
## Constructors

```c#
Gradient( ColorFrame[] frames) 
```
No Summary
```c#
Gradient( ) 
```
No Summary
## Properties

```c#
ImmutableList<AlphaFrame> Alphas { get; set; } 
```
A list of color stops, which should be ordered by time
```c#
BlendMode Blending { get; set; } 
```
The blend mode
```c#
ImmutableList<ColorFrame> Colors { get; set; } 
```
A list of color stops, which should be ordered by time
## Methods

```c#
int AddAlpha( float x, float alpha) 
```
Add an alpha position
```c#
int AddAlpha( in AlphaFrame keyframe) 
```
No Summary
```c#
int AddColor( float x, in Color color) 
```
Add a color position
```c#
int AddColor( in ColorFrame keyframe) 
```
Add given keyframe to this curve.
```c#
Color Evaluate( float time) 
```
Evaluate the blend using the time, which is generally between 0 and 1
```c#
void FixOrder( ) 
```
If the lists aren't in time order for some reason, this will fix them. This should really
just be called when serializing, and in every other situation we should assume they're
okay.
```c#
Gradient WithFrames( ImmutableList<ColorFrame> frames) 
```
Make a copy of this with changed keyframes
## Operators

```c#
ColorFrame this[ int index, ] 
```
No Summary
```c#
implicit Gradient =( Color value) 
```
No Summary
## Nested Types

## Referencing Members

```c#
static void GradientEditorWidget.OpenPopup( Widget, Gradient, Action<Gradient> ) 
```
```c#
Gradient = GradientEditorWidget.Value { get; set; } 
```
```c#
Action<Gradient> = GradientEditorWidget.ValueChanged { get; set; } 
```
