# MathX

## Is static
Derives from object

## Summary

A class to add functionality to the math library that System.Math and System.MathF don't provide.
A lot of these methods are also extensions, so you can use for exampleint i = 1.0f.FloorToInt();
## Methods

```c#
static bool AlmostEqual( float value, float b, float within = 0.0001) 
```
Returns true if given value is close to given value within given tolerance.
```c#
static float Approach( float f, float target, float delta) 
```
Adds or subtracts given amount based on whether the input is smaller of bigger than the target.
```c#
static int CeilToInt( float f) 
```
Rounds up given float to next integer value.
```c#
static float Clamp( float v, float min, float max) 
```
Clamp a float between 2 given extremes.
If given value is lower than the given minimum value, returns the minimum value, etc.
```c#
static float DegreeToRadian( float deg) 
```
Convert degrees to radians.180 degrees is System.Math.PI (roughly 3.14) radians, etc.
```c#
static float DeltaDegrees( float from, float to) 
```
Difference between two angles in degrees. Will always be between -180 and +180.
```c#
static float DeltaRadians( float from, float to) 
```
Difference between two angles in radians. Will always be between -PI and +PI.
```c#
static float Floor( float f) 
```
Remove the fractional part of given floating point number
```c#
static int FloorToInt( float f) 
```
Remove the fractional part and return the float as an integer.
```c#
static float GradiansToDegrees( float grad) 
```
Convert gradians to degrees.100 gradian is 90 degrees, 200 gradian is 180 degrees, etc.
```c#
static float GradiansToRadians( float grad) 
```
Convert gradians to radians.200 gradian is System.Math.PI (roughly 3.14) radians, etc.
```c#
static float InchToMeter( float inches) 
```
Convert inches to meters.
```c#
static float InchToMilimeter( float inches) 
```
Convert inches to millimeters.
```c#
static float Lerp( float from, float to, float frac, bool clamp = true) 
```
Performs linear interpolation on floating point numbers.
```c#
static float LerpDegrees( float from, float to, float frac, bool clamp = true) 
```
Linearly interpolates between two angles in degrees, taking the shortest arc.
```c#
static float LerpDegreesTo( float from, float to, float frac, bool clamp = true) 
```
Linearly interpolates between two angles in degrees, taking the shortest arc.
```c#
static float LerpInverse( float value, float from, float to, bool clamp = true) 
```
Performs inverse of a linear interpolation, that is, the return value is the fraction of a linear interpolation.
```c#
static float LerpRadians( float from, float to, float frac, bool clamp = true) 
```
Linearly interpolates between two angles in radians, taking the shortest arc.
```c#
static float LerpRadiansTo( float from, float to, float frac, bool clamp = true) 
```
Linearly interpolates between two angles in radians, taking the shortest arc.
```c#
static float LerpTo( float from, float to, float frac, bool clamp = true) 
```
Performs linear interpolation on floating point numbers.
```c#
static float[] LerpTo( float[] from, float[] to, float delta, bool clamp = true) 
```
Performs multiple linear interpolations at the same time.
```c#
static float MeterToInch( float meters) 
```
Convert meters to inches.
```c#
static float NormalizeDegrees( float degree) 
```
Convert angle to between 0 - 360
```c#
static float RadianToDegree( float rad) 
```
Convert radians to degrees.180 degrees is System.Math.PI (roughly 3.14) radians, etc.
```c#
static float Remap( float value, float oldLow, float oldHigh, float newLow = 0, float newHigh = 1) 
```
Remap a float value from a one range to another. Clamps value between newLow and newHigh.
```c#
static float Remap( float value, float oldLow, float oldHigh, float newLow, float newHigh, bool clamp) 
```
Remap a float value from a one range to another
```c#
static int Remap( int value, int oldLow, int oldHigh, int newLow, int newHigh) 
```
Remap an integer value from a one range to another
```c#
static float SmoothDamp( float current, float target, ref float velocity, float smoothTime, float deltaTime) 
```
Smoothly move towards the target
```c#
static float SnapToGrid( float f, float gridSize) 
```
Snap number to grid
```c#
static int SnapToGrid( int f, int gridSize) 
```
Snap number to grid
```c#
static float SphereCameraDistance( float radius, float fieldOfView) 
```
Given a sphere and a field of view, how far from the camera should we be to fully see the sphere?
```c#
static float UnsignedMod( float a, float b) 
```
Does what you expected to happen when you did "a % b"
