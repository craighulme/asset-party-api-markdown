# Screenshot

## Derives from object

## Summary

True if this is a loading screen rather than a regular screenshot
## Constructors

```c#
Screenshot( ) 
```
No Summary
## Properties

```c#
DateTime Created { get; set; } 
```
No Summary
```c#
int Height { get; set; } 
```
No Summary
```c#
bool IsVideo { get; set; } 
```
True if this is a loading screen rather than a regular screenshot
```c#
string Thumb { get; set; } 
```
No Summary
```c#
string Url { get; set; } 
```
No Summary
```c#
int Width { get; set; } 
```
No Summary
## Methods

```c#
string GetThumbUrl( int width, int height) 
```
Return the URL of a thumbnail matching this exact size. For caching reasons it's going to be best if
we can keep this to round number sizes (256, 512 etc) rather than trying to exact fit.
