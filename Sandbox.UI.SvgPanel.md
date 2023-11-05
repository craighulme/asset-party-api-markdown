# SvgPanel

## 
```c#
Derives from Panel
```

## Summary

A generic panel that draws an SVG scaled to size
## Constructors

```c#
SvgPanel( ) 
```
No Summary
## Properties

```c#
string Color { get; set; } 
```
Optional color to draw the SVG with
```c#
string Src { get; set; } 
```
Content path to the SVG file
```c#
override bool HasContent { get; } 
```
OverridesPanel.HasContentIf true, callsPanel.DrawContent.
## Methods

```c#
override void FinalLayout( Vector2 offset) 
```
OverridesPanel.FinalLayoutTakes aUI.LayoutCascadeand returns an outer rect
