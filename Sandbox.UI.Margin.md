# Margin

## Derives from ValueType

## Summary

Represents aRectwhere each side is the thickness of an edge/padding/margin/border, rather than positions.
## Constructors

```c#
Margin( Rect r) 
```
No Summary
```c#
Margin( float uniform) 
```
No Summary
```c#
Margin( float horizontal, float vertical) 
```
No Summary
```c#
Margin( float left, float top, float right, float bottom) 
```
No Summary
```c#
Margin( float? left, float? top, float? right, float? bottom) 
```
No Summary
## Properties

```c#
float Bottom { get; set; } 
```
Thickness of the bottom margin.
```c#
Vector2 EdgeSize { get; } 
```
When the Rect describes edges, this returns the total size of the edges in each direction
```c#
float Height { get; set; } 
```
Height of the inner square contained within the margin.
```c#
float Left { get; set; } 
```
Thickness of the left side margin.
```c#
Vector2 Position { get; set; } 
```
Position of the inner top left corder of the margin/border.
```c#
float Right { get; set; } 
```
Thickness of the right side margin.
```c#
Vector2 Size { get; set; } 
```
Size of the inner square contained within the margin.
```c#
float Top { get; set; } 
```
Thickness of the top margin.
```c#
float Width { get; set; } 
```
Width of the inner square contained within the margin.
## Methods

```c#
Margin EdgeAdd( Margin edges) 
```
Where padding is an edge type rect, will return this rect expanded with those edges.
```c#
Margin EdgeSubtract( Margin edges) 
```
Where padding is an edge type rect, will return this rect expanded with those edges.
## Operators

```c#
Margin +( Margin a, Margin b) 
```
No Summary
```c#
Margin *( Margin a, float b) 
```
No Summary
```c#
Margin *( Margin a, Vector2 b) 
```
No Summary
```c#
implicit Margin =( float value) 
```
No Summary
## Referencing Members

```c#
Margin = Box.Border
```
```c#
Margin = Widget.ContentMargins { get; set; } 
```
```c#
static Rect = Paint.DrawTextBox( Rect, string, Color, Margin, float, TextFlag ) 
```
```c#
Margin = Styles.GetInset( Vector2 ) 
```
```c#
Margin = Styles.GetOutset( Vector2 ) 
```
```c#
Rect = Rect.Grow( Margin ) 
```
```c#
Margin = Box.Margin
```
```c#
Margin = Layout.Margin { get; set; } 
```
```c#
Margin = BaseItemWidget.Margin { get; set; } 
```
```c#
Margin = Box.Padding
```
```c#
Rect = Rect.Shrink( Margin ) 
```
```c#
Margin = MarginProperty.Value { get; set; } 
```
