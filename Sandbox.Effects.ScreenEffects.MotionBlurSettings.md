# MotionBlurSettings

## ```c#
Derives from object
```

## Summary

How many blur samples we should take. The higher this value is the
more expensive it is. This value determines how smooth the blur will be
## Constructors

```c#
MotionBlurSettings( ) 
```
No Summary
## Properties

```c#
int Samples { get; set; } 
```
How many blur samples we should take. The higher this value is the
more expensive it is. This value determines how smooth the blur will be
```c#
float Scale { get; set; } 
```
How strong the motion blur should be.
Smaller values seem to work better here, default value is ~0.05f
