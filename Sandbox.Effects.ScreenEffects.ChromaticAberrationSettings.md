# ChromaticAberrationSettings

## Derives from object

## Summary

The pixel offset for each color channel. These values should
be very small as it's in UV space. (0.004 for example)
X = Red
Y = Green
Z = Blue
## Constructors

```c#
ChromaticAberrationSettings( ) 
```
No Summary
## Properties

```c#
Vector3 Offset { get; set; } 
```
The pixel offset for each color channel. These values should
be very small as it's in UV space. (0.004 for example)
X = Red
Y = Green
Z = Blue
```c#
float Scale { get; set; } 
```
Enable chromatic aberration
