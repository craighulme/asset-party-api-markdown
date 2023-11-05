# Easing

## Is static
Derives from object

## Summary

Easing functions used for transitions. Seehttps://easings.net/for examples.
## Methods

```c#
static float BounceIn( float f) 
```
Bouncy ease in.
```c#
static float BounceInOut( float f) 
```
Bouncy ease in and out.
```c#
static float BounceOut( float f) 
```
Bouncy ease out.
```c#
static float EaseIn( float f) 
```
Quadratic ease in.
```c#
static float EaseInOut( float f) 
```
Exponential ease in and out.
```c#
static float EaseOut( float f) 
```
Quadratic ease out.
```c#
static float ExpoIn( float f) 
```
Exponential ease in.
```c#
static float ExpoInOut( float f) 
```
Exponential ease in and out.
```c#
static float ExpoOut( float f) 
```
Exponential ease out.
```c#
static Function GetFunction( string name) 
```
Get an easing function by name (ie, "ease-in").
If the function doesn't exist we return QuadraticInOut
```c#
static float Linear( float f) 
```
Linear easing function, x=y.
```c#
static float QuadraticIn( float f) 
```
Quadratic ease in.
```c#
static float QuadraticInOut( float f) 
```
Quadratic ease in and out.
```c#
static float QuadraticOut( float f) 
```
Quadratic ease out.
```c#
static float SineEaseIn( float f) 
```
Sine ease in.
```c#
static float SineEaseInOut( float f) 
```
Sine ease in and out.
```c#
static float SineEaseOut( float f) 
```
Sine ease out.
```c#
static bool TryGetFunction( string name, out Function function) 
```
Get an easing function by name (ie, "ease-in").
If the function exists we return true, otherwise return false.
## Nested Types

