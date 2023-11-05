# PlanarReflection

## 
```c#
Derives from ScenePortal
```

## Summary

Creates a bounding mesh model for the water reflection.
This way the water reflection scene will only be rendered when the water is visible in player view
## Constructors

```c#
PlanarReflection( SceneWorld world, BBox renderBounds = null) 
```
No Summary
## Methods

```c#
static Model CreateBoundingMeshModel( BBox renderBounds = null) 
```
Creates a bounding mesh model for the water reflection.
This way the water reflection scene will only be rendered when the water is visible in player view
```c#
static bool IsRenderingReflection( ) 
```
Returns true if the renderer is currently rendering the world using a reflection view
```c#
void OnRender( ) 
```
Update on the render thread
```c#
Matrix ReflectMatrix( Matrix m, Plane plane) 
```
Returns a reflected matrix given a plane ( Reflection normal and distance )
```c#
void Update( Vector3 reflectionOffset, Vector3 reflectionNormal, float clipPlaneOffset = 0) 
```
Updates the reflection information before the render
```c#
void UpdateAspectRatio( ) 
```
Updates the aspect ratio of the reflection to match the view
