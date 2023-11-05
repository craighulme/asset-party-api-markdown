# FGDCurve

## 
```c#
Derives from object
```

## Summary

A helper class to handle 'curve' FGD type.
TOOD: Get rid of in favor of new curve stuff.
## Constructors

```c#
FGDCurve( string kv3data) 
```
No Summary
## Properties

```c#
bool IsValid { get; } 
```
Whether the curve was loaded correctly or not
```c#
Vector2 Maxs { get; } 
```
The top right corner of the curve. Mins and Maxs represent the range of inputs and outputs of the curve function.
```c#
Vector2 Mins { get; } 
```
The bottom left corner of the curve. Mins and Maxs represent the range of inputs and outputs of the curve function.
## Methods

```c#
float Get( float x, bool clamp = true) 
```
The cubic spline function in ranges as defined in Hammer/Asset editor.
```c#
float GetNormalized( float x, bool clamp = true) 
```
The cubic spline function normalized to ranges [0,1] on both input and output.
## Operators

```c#
implicit FGDCurve =( string kv3data) 
```
No Summary
