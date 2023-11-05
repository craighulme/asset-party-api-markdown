# ColorPalette

## 
```c#
Derives from Widget
```

## Summary

Used to store and manipulate a collection of colors.
## Constructors

```c#
ColorPalette( Widget parent = null) 
```
No Summary
## Properties

```c#
List<Color> Options { get; set; } 
```
The colors available in this palette
```c#
Color Value { get; set; } 
```
The selected color in this palette
## Methods

```c#
static void PaintSwatch( Color swatchColor, Rect rect, bool highlight, float radius = 4, bool disabled = false) 
```
No Summary
```c#
protected override void DoLayout( ) 
```
OverridesWidget.DoLayoutCalled to make sure all child panels are in correct positions and have correct sizes.
This is typically called when the size of this widget changes, but there are other cases as well.
