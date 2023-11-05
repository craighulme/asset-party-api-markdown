# VignetteSettings

## 
```c#
Derives from object
```

## Summary

The center of the vignette in relation to UV space. This means
a value of {0.5, 0.5} is the center of the screen
## Constructors

```c#
VignetteSettings( ) 
```
No Summary
## Properties

```c#
Vector2 Center { get; set; } 
```
The center of the vignette in relation to UV space. This means
a value of {0.5, 0.5} is the center of the screen
```c#
Color Color { get; set; } 
```
The color of the vignette or the "border"
```c#
float Intensity { get; set; } 
```
How strong the vignette is. This is a value between 0 -> 1
```c#
float Roundness { get; set; } 
```
How circular or round the vignette is
```c#
float Smoothness { get; set; } 
```
How much fall off or how blurry the vignette is
