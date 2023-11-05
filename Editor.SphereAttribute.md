# SphereAttribute

## Derives from MetaDataAttribute

## Summary

Displays a sphere in Hammer with a radius tied to given property and with given color.
The sphere's radius can be manipulated in Hammer's 2D views. You can have multiple of these.
## Constructors

```c#
SphereAttribute( string variableName, uint color, bool singleSelect = false) 
```
No Summary
```c#
SphereAttribute( string variableName, string color, bool singleSelect = false) 
```
No Summary
```c#
SphereAttribute( string variableName = "radius", byte red = 255, byte green = 255, byte blue = 255, bool singleSelect = false) 
```
No Summary
```c#
SphereAttribute( float radius, byte red = 255, byte green = 255, byte blue = 255, bool singleSelect = false) 
```
No Summary
## Properties

```c#
Color32 Color { get; set; } 
```
No Summary
```c#
bool IsLean { get; set; } 
```
If set to true, the sphere will appear as 3 circles in 3D view, rather than a wireframe sphere.
```c#
bool SingleSelect { get; set; } 
```
No Summary
```c#
string VariableName { get; set; } 
```
No Summary
## Methods

```c#
override void AddHelpers( List<Tuple<string, string[]>> helpers) 
```
OverridesMetaDataAttribute.AddHelpers
