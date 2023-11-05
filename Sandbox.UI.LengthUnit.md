# LengthUnit

## Derives from Enum

## Summary

Possible units for various CSS properties that require length, used byUI.Lengthstruct.
## Fields

```c#
static LengthUnit Auto = 0
```
The layout engine will calculate and select a width for the specified element.
```c#
static LengthUnit Center = 11
```
In the middle of the parent at the appropriate axis.
```c#
static LengthUnit Contain = 9
```
For background images, contain the image within the element bounds.
```c#
static LengthUnit Cover = 8
```
For background images, cover the entire element with the image, stretcing and cropping as necessary.
```c#
static LengthUnit End = 10
```
End of the parent at the appropriate axis.
```c#
static LengthUnit Percentage = 2
```
The length is a percentage (0-100) of the parent's length. (typically)
```c#
static LengthUnit Pixels = 1
```
The length is in pixels.
```c#
static LengthUnit Start = 7
```
Start of the parent at the appropriate axis.
```c#
static LengthUnit Undefined = 12
```
Similar to CSS 'unset', basically means we don't have a value; should only really be used under certain
circumstances (e.g. to handle background sizing properly).
```c#
static LengthUnit ViewHeight = 3
```
The length is a percentage (0-100) of the viewport's height.
```c#
static LengthUnit ViewMax = 6
```
The length is a percentage (0-100) of the viewport's largest side/edge.
```c#
static LengthUnit ViewMin = 5
```
The length is a percentage (0-100) of the viewport's smallest side/edge.
```c#
static LengthUnit ViewWidth = 4
```
The length is a percentage (0-100) of the viewport's width.
## Referencing Members

```c#
LengthUnit = Length.Unit
```
