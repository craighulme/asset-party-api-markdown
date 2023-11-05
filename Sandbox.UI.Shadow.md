# Shadow

## ```c#
Derives from ValueType
```

## Summary

Shadow style settings
## Fields

```c#
float Blur
```
Amount of blurring for the shadow.
```c#
Color Color
```
Color of the shadow.
```c#
float OffsetX
```
Shadow offset on the X axis.
```c#
float OffsetY
```
Shadow offset on the Y axis.
```c#
float Spread
```
Increases the box size by this much before starting shadow blur.
Box shadows only.
## Methods

```c#
Shadow LerpTo( Shadow shadow, float delta) 
```
Perform linear interpolation between 2 shadows.
```c#
Shadow Scale( float f) 
```
Scale all variables by given scalar.
```c#
override int GetHashCode( ) 
```
OverridesValueType.GetHashCode
