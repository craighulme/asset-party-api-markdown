# SvgDocument

## Derives from object

## Summary

Helper class for reading Scalable Vector Graphics files.
## Properties

```c#
IReadOnlyList<SvgPath> Paths { get; } 
```
List of all shapes in the document.
## Methods

```c#
static SvgDocument FromString( string contents) 
```
Reads an SVG document from the given string, returning a list of path elements
describing the shapes in the image.
