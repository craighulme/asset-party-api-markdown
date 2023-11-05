# GizmoDraw

## ```c#
Derives from object
```

## Summary

Contains functions to add objects to the Gizmo Scene. This
is an instantiable class so it's possible to add extensions.
## Properties

```c#
Color Color { get; set; } 
```
The color to render the next object
```c#
bool IgnoreDepth { get; set; } 
```
Ignore depth when drawing, draw on top of everything
```c#
float LineThickness { get; set; } 
```
The thickness of line drawings
## Methods

```c#
void Line( in Vector3 a, in Vector3 b) 
```
Draw a line from a to b
```c#
void Line( in Line line) 
```
Draw a line from a to b
```c#
void LineBBox( in BBox box) 
```
Draw a bounding box
```c#
void LineCapsule( Capsule capsule, int rings = 12) 
```
No Summary
```c#
void LineCircle( in Vector3 center, float radius, float startAngle = 0, float totalDegrees = 360, int sections = 16) 
```
Draw a sphere made out of lines
```c#
void LineCylinder( Vector3 vPointA, Vector3 vPointB, float flRadiusA, float flRadiusB, int nNumSegments) 
```
A cylinder
```c#
void LineNavigationMesh( NavigationMesh mesh) 
```
A Navigation Mesh. This will draw each triangle in the mesh.
```c#
void Lines( in IEnumerable<Line> lines) 
```
Draw a lines
```c#
void LineSphere( in Vector3 point, in float radius, in int rings = 8) 
```
Draw a sphere made out of lines
```c#
void LineSphere( in Sphere sphere, int rings = 8) 
```
Draw a sphere made out of lines
```c#
void LineTriangle( in Triangle triangle) 
```
A triangle
```c#
void LineTriangles( in IEnumerable<Triangle> triangles) 
```
Multiple triangles
```c#
SceneObject Model( string modelName, Transform localTransform) 
```
Draw a model
```c#
void Model( string modelName) 
```
Draw a model
```c#
SceneObject Model( Model model, Transform localTransform) 
```
Draw a model
```c#
void Model( Model modelName) 
```
Draw a model
```c#
void Particles( string modelName, Transform localTransform, float? updateSpeed = null) 
```
Draw particles. Control points will be set to the transform position.
```c#
void Particles( string modelName, float? updateSpeed = null) 
```
Draw particles. Control point 0 will be set to the transform position.
```c#
void Plane( Vector3 position, Vector3 normal) 
```
Draw a plane
```c#
void ScreenBiasedHalfCircle( Vector3 center, float radius) 
```
Draws a half circle that tries its best to point towards the camera. This is used by
the rotation widgets that bias towards the camera.
```c#
void ScreenText( string text, Vector2 pos, string font = "Roboto", float size = 12, TextFlag flags = 132) 
```
Draw text
```c#
void SolidBox( BBox box) 
```
Draw a solid box shape
```c#
void SolidCapsule( Vector3 start, Vector3 end, float radius, int hSegments, int vSegments) 
```
Draw a solid capsule shape
```c#
void SolidCircle( Vector3 center, float radius, float startAngle = 0, float totalDegrees = 360, int sections = 8) 
```
Draw a filled circle
```c#
void SolidCone( Vector3 base, Vector3 extent, float flRadius, int? segments = null) 
```
Draw a solid cone shape
```c#
void SolidCylinder( Vector3 start, Vector3 end, float radius, int hSegments = 32) 
```
Draw a solid cylinder shape
```c#
void SolidNavigationMesh( NavigationMesh mesh) 
```
A navigation mesh, will draw the mesh itself solid using the current color.
```c#
void SolidRing( Vector3 center, float innerRadius, float outerRadius, float startAngle = 0, float totalDegrees = 360, int sections = 8) 
```
Draw a filled ring
```c#
void SolidSphere( Vector3 center, float radius, int hSegments = 8, int vSegments = 8) 
```
Draw a solid sphere shape
```c#
void SolidTriangle( in Triangle triangle) 
```
Draw a solid triangle shape
```c#
void SolidTriangle( in Vector3 a, in Vector3 b, in Vector3 c) 
```
Draw a solid triangle shape
```c#
void SolidTriangles( in IEnumerable<Triangle> triangles) 
```
Multiple solid triangles
```c#
void Sprite( Vector3 center, float size, string texture) 
```
No Summary
```c#
void Sprite( Vector3 center, float size, Texture texture) 
```
Draw a sprite. This is horrible right now because it doesn't seem like we can load png textures from disk!?!?
```c#
void Sprite( Vector3 center, Vector2 size, Texture texture, bool worldspace) 
```
Draw a sprite. This is horrible right now because it doesn't seem like we can load png textures from disk!?!?
```c#
void Text( string text, Transform tx, string font = "Roboto", float size = 12, TextFlag flags = 132) 
```
Draw text
```c#
void WorldText( string text, Transform tx, string font = "Roboto", float size = 12, TextFlag flags = 132) 
```
No Summary
