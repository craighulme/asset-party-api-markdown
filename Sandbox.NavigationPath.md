# NavigationPath

## 
```c#
Derives from object
```

## Summary

The individual segments of the path
## Constructors

```c#
NavigationPath( NavigationMesh navigationMesh) 
```
No Summary
## Fields

```c#
List<Segment> Segments
```
The individual segments of the path
## Properties

```c#
bool AllowPathSimplify { get; set; } 
```
When enabled (default) will remove path nodes that are very close to each other.
```c#
bool AllowPathSmoothing { get; set; } 
```
When enabled (default) will smooth the path out
```c#
Vector3 EndPoint { get; set; } 
```
Goal position
```c#
double GenerationMilliseconds { get; set; } 
```
How manuy milliseconds the last geneation took
```c#
Vector3 StartPoint { get; set; } 
```
Start position
## Methods

```c#
protected virtual float ScoreFor( in Connection connection, Vector3 position) 
```
Get the score for this area
```c#
void Build( ) 
```
Build the path. Plenty of opportunity for optimization here.
```c#
Vector3 GetPositionAlongPath( float distance) 
```
No Summary
## Nested Types

