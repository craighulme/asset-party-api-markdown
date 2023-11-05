# Curve

## ```c#
Derives from ValueType
```

## Summary

Describes a curve, which can have multiple key frames.
## Constructors

```c#
Curve( List<Frame> frames) 
```
No Summary
```c#
Curve( Frame[] frames) 
```
No Summary
```c#
Curve( ) 
```
No Summary
## Fields

```c#
ImmutableList<Frame> Frames
```
A list of keyframes or points on the curve.
## Properties

```c#
int Length { get; } 
```
Amount of key frames or points on the curve.
```c#
Vector2 TimeRange { get; set; } 
```
The range of this curve. This affects looping.
```c#
Vector2 ValueRange { get; set; } 
```
The value range. This should affect nothing but what it looks like in the editor.
## Methods

```c#
int AddPoint( float x, float y) 
```
Add a new keyframe at given position to this curve.
```c#
int AddPoint( in Frame keyframe) 
```
Add given keyframe to this curve.
```c#
float Evaluate( float time) 
```
Returns the value on the curve at given time position.
```c#
float EvaluateDelta( float time) 
```
Like evaluate but takes a normalized time between 0 and 1 and returns a normalized value between 0 and 1
```c#
void Fix( ) 
```
If the curve is broken in some way, we can fix it here.
Ensures correct time and value ranges, and that the curve has at least one point.
```c#
Curve WithFrames( ImmutableList<Frame> frames) 
```
Make a copy of this curve with changed keyframes
## Operators

```c#
Frame this[ int index, ] 
```
No Summary
```c#
implicit Curve =( float value) 
```
No Summary
## Nested Types

## Referencing Members

```c#
CurveEditorPopup.CurveEditorPopup( Widget, Curve ) 
```
```c#
Action<Curve> = CurvePresets.OnCurveClicked { get; set; } 
```
```c#
Action<Curve> = CurveEditorPopup.OnValueChanged { get; set; } 
```
```c#
Curve = CurveEditorPopup.Value { get; set; } 
```
```c#
Curve = Curve2DProperty.Value { get; set; } 
```
```c#
Curve = EditableCurve.Value { get; set; } 
```
