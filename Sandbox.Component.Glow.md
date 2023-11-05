# Glow

## Derives from EntityComponent<ModelEntity>

## Summary

A component for controlling the "glow" outline on a entity
## Constructors

```c#
Glow( ) 
```
No Summary
## Properties

```c#
Color Color { get; set; } 
```
The colour of the glow outline
```c#
Color InsideColor { get; set; } 
```
Color of the inside of the glow
```c#
Color InsideObscuredColor { get; set; } 
```
Color of the inside of the glow when the mesh is obscured by something closer.
```c#
Material Material { get; set; } 
```
If defined, the glow will use this material rather than a generated one.
```c#
Color ObscuredColor { get; set; } 
```
The colour of the glow when the mesh is obscured by something closer.
```c#
float Width { get; set; } 
```
The width of the line of the glow
