# RenderState

## Derives from ValueType

## Summary

Describes panel's position and size for rendering operations.
## Properties

```c#
float Height { get; init; } 
```
Height of the panel.
```c#
float Width { get; init; } 
```
Width of the panel.
```c#
float X { get; init; } 
```
Position of the panel on the X axis. This can be a negative value!
```c#
float Y { get; init; } 
```
Position of the panel on the Y axis. This can be a negative value!
## Operators

```c#
implicit Rect =( RenderState rs) 
```
No Summary
