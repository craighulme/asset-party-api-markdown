# Box

## Derives from object

## Summary

Represents position and size of aUI.Panelon the screen.
## Constructors

```c#
Box( ) 
```
No Summary
## Fields

```c#
Margin Border
```
The size of border.
```c#
Rect ClipRect
```
Box.Rectminus the border sizes.
Used internally to "clip" (hide) everything outside of these bounds, if the panelsUI.OverflowModeis not set toOverflowMode.Visible.
```c#
Margin Margin
```
The size of border.
```c#
Margin Padding
```
The size of padding.
```c#
Rect Rect
```
Position and size of the element on the screen,including its padding, but not margin.
```c#
Rect RectInner
```
Position and size of only the element's inner content on the screen, without padding OR margin.
```c#
Rect RectOuter
```
Position and size of the element on the screen,including both - its padding AND margin.
## Properties

```c#
float Bottom { get; } 
```
Position of the bottom edge in screen coordinates.
```c#
float Left { get; } 
```
Position of the left edge in screen coordinates.
```c#
float Right { get; } 
```
Position of the right edge in screen coordinates.
```c#
float Top { get; } 
```
Position of the top edge in screen coordinates.
