# MaskMode

## ```c#
Derives from Enum
```

## Summary

Possible values formask-modeCSS property.
## Fields

```c#
static MaskMode Alpha = 1
```
The alpha channel values of the mask layer image should be used as the mask values.
```c#
static MaskMode Luminance = 2
```
The luminance values of the mask layer image should be used as the mask values.
```c#
static MaskMode MatchSource = 0
```
If the mask-image property is of type 'mask-source', the luminance values of the mask layer image should be used as the mask values.
If it is of type 'image', the alpha values of the mask layer image should be used as the mask values.
## Referencing Members

```c#
MaskMode? = BaseStyles.MaskMode { get; set; } 
```
